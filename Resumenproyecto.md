**Nuclear single-copy nuclear genes (SCNG) identification in transcriptome of A. tequila and A. deserti for Phylogenetics analises**

En filogenética uno de los mayores problemas es la obtención de secuencias con suficiente variación para una correcta delimiación de los clados y así establecer diferentes categorias taxonómicas. Existen grupos de reciente diversificación y/o con eventos de especiación los cuales debido al poco tiempo que han tenido para diferenciarse genéticamente, los marcadores universales no aportan suficiente variación y por ende muy baja resolución a la filogenia del grupo. _Agave s.l_ es un ejemplo de este caso, el grupo divirgió hace 10 m.a y presenta dos momentos de especiación uno hace 8 m.a relacionado con la adaptación y colonizacion a los medios áridos y el segundo hace 3 m.a relacionado con los sindromes de polinización (Good-Avila et al., 2006). Estos recientes eventos hacen que la variacion presente en los marcadores universales de cloroplasto y nucleares sea insuficiente para conocer la historia evolutiva del género _Agave s.l._ 

Los SCNG son más variables, presentan una mayor cantidad de caracteres parsimoniosamente informativos y presentan información biparental, en comparación con los marcadores de cloroplasto. Cuando los genes nucleares presentan una baja cantidad de copias se convierten en un recurso valioso para la identificación de loci ortológos, es decir aquellos loci homólogos que derivan a partir de un evento de especiación, los cuales pueden ser útiles en el desarrollo de estudios filogenómicos (Granados-Mendoza et al., 2015). Por ello el objetivo del presente trabajo es la identificación de genes nucleares con altos valores de variación que nos permitan una mayor resolución filogenética. El método de Smet para la identificación de SCNG consiste en la comparación de transcriptomas a partir de una base de datos de genes resistentes a la duplicacion en 17 angiospermas realizada por Smet et al., (2013). También, la base de datos se compone por los grupos de genes ortológos de la base de datos de PLAZA 2.5 (Van Bel et al. 2011) y OrthoMCL (Li et al. 2003). Esta comparación se clasifica en dos modalidad "Strictly" si se encuentra una sola copia en todas las especies o "Mostly" si se encuentra ducplicado en una o más especies. Dentro de la base de datos de Smet et al., (2013) se cuenta con genomas la familia Amarillydaceae, una de las familias mas cercanas a la Asparagaceae en donde se encuentra el género _Agave_ por lo cual se consideró que la busqueda de genes ortológos sería más eficiente al tener modelos cercanos a la especie de estudio.  


**Methods** 

La identificación de genes nucleares que aporten resolución a la filogenia del género _Agave s.l_ se realizó por el método de Smet en el cual se realiza una comparacion de un transcriptoma con una base de datos de genes ortológos y se clasifica en "Strictly" cuando solo existe una copia en todas las especies comparadas o "Mostly" cuando existe una duplicación en una o más de las especies comparadas. Para los análisis se descargaron los transcriptomas de dos especies de Agave de la base de datos de Dryad. Las especies fueron _Agave deserti_ y _Agave tequilana_, se realizó una busqueda sin emnargo, no existe ningun genoma publicado de Agave y solo existen dos transcriptomas. Una vez descargados los transcriptomas se procedio a hacer las correcciones pertinentes para generar los input para el análisis. 

La busqueda de genes ortológos se realizó en el software Markerminer v. 1.2 (Chamala et al., 2015) mediante instrucciones en linea de comando. Se emplearón los valores establecidos por default y se seleccionó a la especie Arabidopsis Thaliana como modelo. Una vez terminado el análisis de los transcriptomas a partir del output que contenia la información de los genes nucleares encontrados se realizó una gráfica empleando ggplot2 en Rstudio con la finalidad de realizar una comparación en el número de ortológos encontrados en cada gen.

**Results** 

A partir de los transcriptomas de A. deserti y A.tequilana se obtuvieron un total de 13 genes nucleares de los cuales  12 se encuentran en la categoria de "Mostly" y solo uno en la categoria "Stricly" por otra parte se analizaron los genes encontrados evaluando el número de ortólogos presentes en cada uno de los genes (fig.1) con la finalidad de seleccionar aquellos genes que son de copia unica y que tienen el mayor número de ortólogos. La mayor parte de los genes corresponden a la familia de las cinasas mientras que el único gen con la categoria de "Stricly" pertenece a la familia de proteinas de las Pentatricopeptide y se localiza en la mitocondria.

![Genes Ortólogos](https://github.com/Ofeabi/ProyectoFinalBioinf2017-II/blob/master/GraphSCNG.png "Genes Ortológos")

**Analysis and Conclusion** 

En la actualidad existen diversos métodos para la detección de genes que nos aportan mayor resolución en las filogenias. Sin embago, la tecnología y  métodos cambian continuamente y cada investigador debe seleccionar el mejor método con base en su criterio. En el caso de Markerminer es un software que a pesar de haber sido generado en el 2015 aun no cuenta con suficiente difusión por lo que los trabajos en los que se ha empleado son escasos. Aunque, cuenta con una amplia guía para la instalación y generación de la linea de comando para correrlo así como direcciones de correo electrónico en las cuales mantienen la disposición para orientar a los usuarios. Además, cuentan con un reposositorio en donde se explica detalladamente la manera en que funciona Markerminer para la detección de genes ortólogos de copia unica. Los output que genera son muy claros y se generan en formatos que son compatibles para muchos otros softwares como txt, fasta o phy. 

En cuanto a la información que se genera puede funcionar como un primer aproximamiento en la detección de genes que pueden aportar resolución al género _Agave_. Sin embargo, las bases de datos que a partir de las cuales se genera la comparación y busqueda es pequeña. Es probable que al agregar una mayor cantidad de transcriptomas en el análisis aporte una mayor cantidad de genes específicos para los Agaves. También, es necesario realizar pruebas con los valores de similitud de las proteínas, longitud minima de los transcritos, modelo de referencia y el porcentaje minimo de cobertura del transcrito se pueden realizar filtros más o menos estrictos con la finalidad de encontrar genes que aporten mayor resolución.         

**Conclusión con respecto a la materia** 

A pesar de haber tenedo muchas dificultades con la instalación mediante la línea de comando y tener que googlear miles de dudas  debo admitir que la materia me ayudo bastante ya que al iniciar el curso no tenia la más minima idea de como hacer las cosas o que googlear para aprender a hacerlo. Me siento santisfecha con lo que he avanzado pues pase de pensar que nunca podría hacer una gráfica o plottear un mapa para mi artículo a pensar que puedo hacerlo y que tengo las bases para realizar una busqueda en foros, vigenetts, manuales o diversos materiales que me permitirán realizarlo. La bioinformática es una constante tarea de pensar en lo que quieres, como realizarlo, buscar, preguntar, googlear, intentarlo, frustrarte, volver a intentar y lograrlo.     


**Literature** 

Chamala, S., García, N., Godden, G. T., Krishnakumar, V., Jordon-Thaden, I. E., De Smet, R., Barbazuk, W. B., Soltis, D. E., and Soltis, P. S. 2015. MarkerMiner 1.0: A new application for phylogenetic marker development using angiosperm transcriptomes Applications in Plant Sciences 3(4): 1400115.

De Smet, R., K.L. Adams, K. Vandepoele, M.C.E. Van Montagu, S. Maere, and Y. Van de Peer. 2013. Convergent gene loss following gene and genome duplications creates single-copy families in flowering plants. Proceedings of the National Academy of Sciences 110: 2898–2903.

Gross, S. M., Martin, J. A., Simpson, J., Abraham-Juarez, M. J., Wang, Z., & Visel, A. (2013). De novo transcriptome assembly of drought tolerant CAM plants, Agave deserti and Agave tequilana. BMC genomics, 14(1), 563.

Li, L., C.J. Stoeckert, and D.S. Roos. 2003. OrthoMCL: identification of ortholog groups for eukaryotic genomes. Genome research 13: 2178–2189.

Mendoza, C. G., Naumann, J., Samain, M. S., Goetghebeur, P., De Smet, Y., & Wanke, S. (2015). A genome-scale mining strategy for recovering novel rapidly-evolving nuclear single-copy genes for addressing shallow-scale phylogenetics in Hydrangea. BMC evolutionary biology, 15(1), 132.

Van Bel, M., S. Proost, E. Wischnitzki, S. Movahedi, C. Scheerlinck, Y. Van de Peer, and K. Vandepoele. 2011. Dissecting plant genomes with the PLAZA comparative genomics platform. Plant Physiology, pp–111.






