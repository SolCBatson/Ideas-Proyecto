# SCRIPT 
## Programa 
* Programa utilizado NCBI_NUCLEOTIDE.sh de Raul OG 
* Editamos y borramos la línea de rm tmp_sequences.gb
* bash NCBI_NUCLEOTIDE.sh -t Viperidae -m PLA2 -o rmViperidae.fasta
* cat tm tmp_sequences.gb
* grep "geo_loc" tmp_sequences.gb
* /geo_loc_name="Viet Nam"
  *                   /geo_loc_name="Viet Nam"
   *                  /geo_loc_name="China: Sichuan Province"
    *                 /geo_loc_name="China: Sichuan Province"
     *                /geo_loc_name="Japan:Okinawa, Kume island"
      *               /geo_loc_name="Japan:Okinawa, Iheya island"
       *              /geo_loc_name="Peru"
        *             /geo_loc_name="Tunisia:South Tunisia"
         *            /geo_loc_name="Japan:Okinawa, The Sakaishima Islands"
          *           /geo_loc_name="Japan:Okinawa, The Sakaishima Islands"
           *          /geo_loc_name="Japan:Okinawa, The Sakishima Islands"
            *         /geo_loc_name="Japan:Okinawa"
* Borramos innecesario
* rm rmViperidae.fasta 
## Para la filogenia
* Ya sabemos las locaciones  
* Repetimos esto con cada locación 
* bash NCBI_NUCLEOTIDE.sh -t Viperidae -l Japan -m PLA2 -o Viperidae_Japan.fasta
* count=1; while read -r line; do if [[ "$line" =~ ^\> ]]; then echo ">JP$count ${line#* }"; ((count++)); else echo "$line"; fi; done < Viperidae_Japan.fasta > Japan_viperidae_pla2.fasta
* cat Japan_viperidae_pla2.fasta
## Unir documentos
cat *.fasta > Viperidae_geo.fasta
## Alinear 
* ./muscle3.8.31_i86linux64 -in Viperidae_geo.fasta -out muscle_viperidae_locations.fasta                 -maxiters 1 -diags
* Me descargo en la computadora 
* scp dechavez@hoffman2.idre.ucla.edu:/u/scratch/d/dechavez/Bioinformatica-PUCE/RediseBio/SolCB/Proyecto/Proyect/muscle_viperidae_geo.fasta ./
## Atom
* >(\w+)\s+(\w+)\s+(\w+).*
* >$1_$2_$3
* Subir a hoffman
* scp aligned_viperidae_locations.fasta dechavez@hoffman2.idre.ucla.edu:/u/scratch/d/dechavez/Bioinformatica-PUCE/RediseB
io/SolCB/Proyecto/Proyect
## Iqtree
* module load iqtree/2.2.2.6
* iqtree2 -s aligned_viperidae_locations.fasta
* Descargarme en mi computadora
* scp dechavez@hoffman2.idre.ucla.edu:/u/scratch/d/dechavez/Bioinformatica-PUCE/RediseBio/SolCB/Proyecto/Proyect/aligned_viperidae_locations.fasta.treefile ./
## Figtree
* Abrimos el documento .treefile en Figtree
