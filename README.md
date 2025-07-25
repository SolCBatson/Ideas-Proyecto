# Proyecto 
## Nombre de tu proyecto
Filogenia Molecular de Viperidae mediante Secuencias de Fosfolipasas A2 (PLA2) del Veneno

## Autores del proyecto
Sol Castro

## Propósito del programa de tu proyecto
Este proyecto busca reconstruir las relaciones filogenéticas dentro de la familia Viperidae utilizando secuencias de proteínas fosfolipasas A2 (PLA2) y observar evolución molecular de estas toxinas en diferentes linajes de víboras. Las PLA2 son las principales responsables de los efectos miotóxicos y neurotóxicos observados en el envenenamiento por serpientes. Provocan daño tisular local, edema y efectos sistémicos como la rabdomiólisis (De Oliveira et al., 2024). Los efectos inflamatorios de las PLA2 se producen a través de la liberación de eicosanoides, que son potentes mediadores inflamatorios. Esto es evidente en los venenos de serpientes bothrópicas, que son ortólogos de las PLA2 de los mamíferos (Zuliani et al., 2022). La neurotoxicidad es otro efecto significativo, ya que algunas PLA2 son capaces de bloquear las corrientes provocadas por la acetilcolina, lo que indica su interacción con los receptores nicotínicos de acetilcolina bloqueando la entrada de iones a través de estos canales iónicos (Vulfius et al., 2013).
## Antecedentes
La importancia de estudiar molecularmente los venenos de las serpientes es porque se ha vuelto un gran problema de salud publica en todo el mundo, con tasas de mortalidad anuales de entre 81 000 y 138 000 personas, y muchas más que sufren discapacidades permanentes (Bittenbinder et al., 2023). Las terapias antivenenos actuales suelen ser inadecuadas debido a la complejidad de la composición de los venenos. La caracterización exhaustiva de los venenos puede contribuir al desarrollo de antivenenos más eficaces y diseñados de forma racional (Wang et al., 2024). La investigación de los mecanismos moleculares del daño inducido por el veneno, como la alteración de la membrana y la degradación de la matriz extracelular, es fundamental para mejorar las estrategias de tratamiento (Bittenbinder et al., 2023). El estudio de los venenos de serpiente proporciona información sobre la biología evolutiva, ya que la composición del veneno varía significativamente dentro y entre especies debido a factores bióticos y abióticos (C. F. Smith et al., 2023). Los estudios genómicos de los venenos de serpiente pueden revelar los mecanismos de evolución del veneno, como la duplicación de genes y la selección positiva, que contribuyen a la diversificación del veneno (Rao et al., 2022). Comprender los factores evolutivos que impulsan la variación del veneno puede servir de base para el diseño de antídotos y otros agentes terapéuticos (Rao et al., 2022; C. F. Smith et al., 2023).

![Alt text](https://cdn.agenciasinc.es/var/ezwebin_site/storage/images/_aliases/img_1col/noticias/asi-evoluciono-el-veneno-de-las-cobras-escupidoras-como-mecanismo-de-defensa/8557053-4-esl-MX/Asi-evoluciono-el-veneno-de-las-cobras-escupidoras-como-mecanismo-de-defensa.jpg) 

## Datos 
Los datos se descargarán de NCBI de las secuencias de las proteínas fosfolipasas A2 (PLA2) de toda la familia viperidae.
## Metodología
Con los datos adquiridos previamente en formato fasta se utilizarán los siguientes programas en Git BASH: 
<<<<<<< HEAD
* Se descargarán los archivos para poder modificarlos en Atom
* Atom: Eliminar datos innecesarios para que solo este el nombre científico
* Subir los documentos a la supercomputadora 
* Muscle: Alinear las secuencias  
* Iqtree: Realizar las Filogenias 
* Descargar el documento .tree 
* Visualizar la filogenia final en FigTree.

## Resultados 
![Filogenia](RESULTS/Filogenia_Viperidae_PLA2)
* Fig.1 La relación filogenética de la proteína PLA2 en Viperidae
* El grupo externo: Naja naja 
* La procedencia geográfica:
* CH = China
* PE = Perú
* IN = India
* JP = Japón
* TU = Túnez
* VM = Vietnam
El árbol filogenético obtenido para la secuencia del gen PLA2 en miembros de la familia Viperidae, con Naja naja como grupo externo, revela una fuerte influencia de la distribución geográfica en la divergencia genética, incluso dentro de una misma especie. A lo largo del árbol, se observa que secuencias correspondientes a especies idénticas —como Protobothrops flavoviridis o Bothrops atrox— aparecen agrupadas en clados distintos, dependiendo del país de origen, lo que sugiere variación intraespecífica significativa.
Por ejemplo, P. flavoviridis presenta agrupamientos separados para secuencias procedentes de Japón (JP) y China (CH), indicando una posible divergencia geográfica relacionada con el aislamiento insular o diferencias ecológicas regionales. De manera similar, B. atrox muestra secuencias de Perú (PE) posicionadas en clados distintos, lo que podría reflejar procesos de diferenciación genética en distintas zonas de la Amazonía.
En términos generales, las secuencias de regiones asiáticas —China (CH), Japón (JP), India (IN) y Vietnam (VM)— no forman un clado monofilético, sino que se distribuyen en varios agrupamientos, lo cual sugiere una historia evolutiva compleja con posibles eventos de dispersión, aislamiento o convergencia funcional del gen PLA2. Por su parte, las secuencias de Túnez (TU) aparecen más claramente separadas, indicando un linaje diferenciado dentro de Viperidae africanos o mediterráneos.
El grupo externo Naja naja, utilizado para enraizar el árbol, se ubica correctamente fuera del clado de Viperidae, confirmando su papel como referencia evolutiva y reforzando la separación filogenética clara entre Elapidae y Viperidae.
En conjunto, la filogenia sugiere que la evolución del gen PLA2 en serpientes Viperidae no está estrictamente asociada a la identidad taxonómica, sino que se ve modulada por la procedencia geográfica, apoyando la existencia de variación genética regional o linajes crípticos dentro de ciertas especies.

## Conclusiones 
Los resultados filogenéticos demuestran que la variedad genética del gen PLA2, responsable de una de las principales toxinas del veneno de serpientes Viperidae, puede variar significativamente incluso entre individuos de una misma especie que habitan en diferentes regiones de un mismo país. Esta divergencia intraespecífica sugiere que las poblaciones locales de serpientes pueden tener composiciones de veneno distintas, lo que tiene implicaciones críticas para la salud pública.
En particular, esta variabilidad podría afectar la eficacia de los antivenenos, los cuales suelen desarrollarse a partir del veneno de unas pocas poblaciones o especies representativas. La existencia de linajes crípticos o variantes geográficas no contempladas en la producción de antiofídicos podría reducir su efectividad en casos reales de mordedura.
Por tanto, este estudio resalta la importancia de considerar la diversidad genética intraespecífica en estudios toxicológicos y médicos, y destaca la necesidad de no generalizar la identidad de las especies venenosas sin evaluar sus poblaciones regionales, promoviendo un enfoque más localizado y preciso en la investigación y desarrollo de tratamientos antiofídicos.


## Referencias 
Bittenbinder, M. A., Capinha, L., Da Costa Pereira, D., Slagboom, J., Van de Velde, B., Casewell, N. R., Jennings, P., Kool, J., & Vonk, F. J. (2023). Development of a high-throughput in vitro screening method for the assessment of cell-damaging activities of snake venoms. PLoS Neglected Tropical Diseases, 17(8), e0011564. https://doi.org/10.1371/journal.pntd.0011564
De Oliveira, A. L. N., Lacerda, M. T., Ramos, M. J., & Fernandes, P. A. (2024). Viper Venom Phospholipase A2 Database: The Structural and Functional Anatomy of a Primary Toxin in Envenomation. Toxins, 16(2), 71. https://doi.org/10.3390/toxins16020071
Rao, W., Kalogeropoulos, K., Allentoft, M. E., Gopalakrishnan, S., Zhao, W., Workman, C. T., Knudsen, C., Jiménez-Mena, B., Seneci, L., Mousavi-Derazmahalleh, M., Jenkins, T. P., Rivera-De-Torre, E., Liu, S., & Laustsen, A. H. (2022). The rise of genomics in snake venom research: recent advances and future perspectives. GigaScience, 11. https://doi.org/10.1093/gigascience/giac024
Smith, C. F., Nikolakis, Z. L., Ivey, K., Perry, B. W., Schield, D. R., Balchan, N. R., Parker, J., Hansen, K. C., Saviola, A. J., Castoe, T. A., & Mackessy, S. P. (2023). Snakes on a plain: biotic and abiotic factors determine venom compositional variation in a wide-ranging generalist rattlesnake. BMC Biology, 21(1). https://doi.org/10.1186/s12915-023-01626-x
Vulfius, C. A., Gorbacheva, E. V., Starkov, V. G., Kasheverov, I. E., Andreeva, T. V., Osipov, A. V., Tsetlin, V. I., & Utkin, Y. N. (2013). Phospholipases A2 isolated from snake venoms block acetylcholine-elicited currents in identified Lymnaea stagnalis neurons. Biochemistry (Moscow) Supplement Series A Membrane And Cell Biology, 7(3), 203-206. https://doi.org/10.1134/s1990747813040077
Wang, C. R., McFarlane, L. O., & Pukala, T. L. (2024). Exploring snake venoms beyond the primary sequence: From proteoforms to protein-protein interactions. Toxicon, 247, 107841. https://doi.org/10.1016/j.toxicon.2024.107841
Zuliani, J. P., Diniz-Sousa, R., Da Silva Setubal, S., Boeno, C. N., Lopes, J. A., & Zamuner, S. R. (2023). Inflammatory effects of phospholipase A2s present in snake venom of the genus Bothrops. En Elsevier eBooks (pp. 173-196). https://doi.org/10.1016/b978-0-323-95698-7.00009-7

