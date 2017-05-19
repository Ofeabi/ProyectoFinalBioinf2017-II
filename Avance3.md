**AVANCE 3**

El objetivo del proyecto es la identificación de genes nucleares de copia unicos a partir de transcriptomas, los cuales presenten suficiente
variación para la resolución de la filogenia del género Agave s.l. Inicialmente se pensó en el software BUSCO, el cual proporciona una medida cuantitatva
de la calidad del ensamble de transcriptomas, genomas o conjuntos de genes, esta medida la obtiene realizando una comparacion con una base de datos
llamadaba OrthoBD en la cual se encuentran genes ortologos universales de distintos grupos biologicos. Por lo cual creo que al ser universales no presentaran 
mucha variacion para el nivel de especies, ya que se han probado genes universales tales como los ITS y a nivel especie no son suficiente. 

Por esta razon se realizo la busqueda de un software que me ayude a buscar genes mas específicos y encontre MarkerMiner un software que se encarga de buscar
genes nucleres de copia unica a partir de transcriptomas, esto lo hace mediante la comparación con 17 genomas de angiospermas en los cuales se realizo una busqueda
entre los 17 genomas que se encuentran en la base de datos mencionan que se encuentra uno perteneciente a la familia Amaryllidaceae, la cual es cercana a la famalia
Asparagaceae en donde se encuentran los agaves. Lo hace de la siguiente manera: 1) realiza un alineamiento de los transcriptomas y filtra los genes nucleares de copia unica presentes en cada uno de los transcriptomas 
proporcionados, 2) corre cada uno de los genes de copia unica a traves del ensamble, 3) cada uno de los genes encontrados es realineado con MAFFT. Dado que se encontraron dos 
transcriptomas de agave se incluiran los dos, ya que con base en el articulo del software estos analisis aportan mayor robustes cuando se agregan mas transcriptomas
pero se pueden realizar a partir de dos.

HASTA EL MOMENTO:

1. Se han descargado los transcriptomas en formato fasta y se editaron según los requerimientos del software para el input

2. Se descargaron las dependencias necesarias para MarkerMiner 

3. Se instalo el software MarkerMiner y se analizarón cuales son las flags a usar y que parametros incluir en el análisis como por ejemplo 
la covertura que se usara, si se realizara una busqueda "Strictly" o "Mostly" y el grupo taxonomico base el analisis

4. se realizo un borrador de la linea de comando a utilizar con base en las decisiones tomadas de los parametros y flags a emplear

5. Se reviso el manual para entender cuales son los output que se obtendran y poder analizarlos de manera correcta

6. El proyecto ya se encuentra organizado por carpetas, se ha avanzado en el resumen markdown, se ha avanzado en los srcipts (en el cual se incluira el de 
instalacion del programa debido a que a pesar de ser muy destalladas las instrucciones se tuvieron que realizar unos cambios para algunas de las paqueterias) y 
ha avanzado en el [README](https://github.com/Ofeabi/ProyectoFinalBioinf2017-II/blob/master/Avance3README). 

FALTA POR HACER

1. Correr el borrador de la linea de comando con los parametros seleccionados

2. analizar los output del programa

3. realizar una grafica de los genes encontrados en Rstudio o ggplot 

