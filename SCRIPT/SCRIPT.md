* esearch -db nucleotide -query "PLA2[Gene] AND Naja naja[Organism]" | \ efetch -format fasta > pla2_naja_naja.fasta
* count=1; while read -r line; do if [[ "$line" =~ ^\> ]]; then echo ">IN$count ${line#* }"; ((count++)); else echo "$line"; fi; done < naja_naja_India.fasta > India_Naja_naja_pla2.fasta
* nano NCBI_NUCLEOTIDE.sh 
* bash NCBI_NUCLEOTIDE.sh -t Viperidae -m PLA2 -o rmViperidae.fasta
* grep "geo_loc" tmp_sequences.gb
* rm rmViperidae.fasta
* bash NCBI_NUCLEOTIDE.sh -t Viperidae -l Japan -m PLA2 -o Viperidae_Japan.fasta
* bash NCBI_NUCLEOTIDE.sh -t Viperidae -l Viet -m PLA2 -o Viperidae_Vietnam.fasta
* bash NCBI_NUCLEOTIDE.sh -t Viperidae -l China -m PLA2 -o Viperidae_China.fasta
* bash NCBI_NUCLEOTIDE.sh -t Viperidae -l Peru -m PLA2 -o Viperidae_Peru.fasta
* bash NCBI_NUCLEOTIDE.sh -t Viperidae -l Tunisia -m PLA2 -o Viperidae_Tunisia.fasta
* count=1; while read -r line; do if [[ "$line" =~ ^\> ]]; then echo ">JP$count ${line#* }"; ((count++)); else echo "$line"; fi; done < Viperidae_Japan.fasta > Japan_viperidae_pla2.fasta
* count=1; while read -r line; do if [[ "$line" =~ ^\> ]]; then echo ">VM$count ${line#* }"; ((count++)); else echo "$line"; fi; done < Viperidae_Vietnam.fasta > Vietnam_viperidae_pla2.fasta
* count=1; while read -r line; do if [[ "$line" =~ ^\> ]]; then echo ">CH$count ${line#* }"; ((count++)); else echo "$line"; fi; done < Viperidae_China.fasta > China_viperidae_pla2.fasta
* count=1; while read -r line; do if [[ "$line" =~ ^\> ]]; then echo ">PE$count ${line#* }"; ((count++)); else echo "$line"; fi; done < Viperidae_Peru.fasta > Peru_viperidae_pla2.fasta
* count=1; while read -r line; do if [[ "$line" =~ ^\> ]]; then echo ">TU$count ${line#* }"; ((count++)); else echo "$line"; fi; done < Viperidae_Tunisia.fasta > Tunisia_viperidae_pla2.fasta
* cat *pla2.fasta > Viperidae_geo.fasta
* ./muscle3.8.31_i86linux64 -in Viperidae_geo.fasta -out muscle_viperidae_locations.fasta                 -maxiters 1 -diags
* scp dechavez@hoffman2.idre.ucla.edu:/u/scratch/d/dechavez/Bioinformatica-PUCE/RediseBio/SolCB/Proyecto/Proyect/muscle_viperidae_geo.fasta ./
* scp aligned_viperidae_locations.fasta dechavez@hoffman2.idre.ucla.edu:/u/scratch/d/dechavez/Bioinformatica-PUCE/RediseBio/SolCB/Proyecto/Proyect
* module load iqtree/2.2.2.6 
* iqtree2 -s aligned_viperidae_locations.fasta
* scp dechavez@hoffman2.idre.ucla.edu:/u/scratch/d/dechavez/Bioinformatica-PUCE/RediseBio/SolCB/Proyecto/Proyect/aligned_viperidae_locations.fasta.treefile ./

