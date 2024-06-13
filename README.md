ESPAÑOL:

Introducción:

Uno de los grandes desafios del país, es controlar la gente y establecer campañas para mejorar la calidad de vida de las personas, las estadísticas que se revisarán recurren al estudio de la poblacion nacional, y la tasa
de natalidad y mortalidad para la población, para conocer el estado actual del País, conocer puntos de inflección, sucesos que pudiesen provocar éstas inflecciones, y sobre todo, soluciones a problematicas que van 
se verán reflejadas en los numeros a venir.

Dentro de la información, podremos dividir el desarrollo en dos grandes ramas:

a) Análisis progresivo del país en cuestión, considerando el desarrollo del indicador a través del tiempo, su progresión a través de la historia y sucesos que pudiesen influir en el cambio

b) Una comparación de las estadísticas con otros países, conocer que diferencias existen, y las posibles mejoras que se pueden imitar de los paises con mejores estadísticas.


Dónde se encuentran éstos Datos?

Éstos datos se encuentran abiertos a todo publico desde https://data.worldbank.org/.

Se extrayeron particularmente desde https://www.kaggle.com/datasets/programmerrdai/global-life-expectancy-at-birth/data, que es una recopilación de la información.


Método de uso:

Desde la entrada 7 podemos observar la lista de todos los indicadores que podemos utilizar para hacer el análisis, para usar el nombre de éstos en los gráficos que queramos.

En la entrada 9 tenemos nuestras listas de indicadores, de los cuales se armarán los gráficos, cada lista corresponde a un gráfico distintos, podemos editar nuestras propias listas desde los indicadores revisados
anteriormente.

Luego en la entrada 10 tenemos la creación de los gráficos, cada gráfico tendrá:
- Como primer argumento el país que se analizará.
- Segundo argumento la lista de indicadores que creamos en el punto anterior.
- Nuestro tercer argumento representa el nombre de nuestro gráfico.
- el ultimo argumento, "numeric" o "porcentage" se refiere a si el gráfico tendrá valores numéricos o en algun porcentaje %.

En la entrada 12 obtendremos nuevos parámetros para ahora analizar distintos paises con el mismo indicador. Se deberán ingresar en este caso dos parámetros, una lista con los paises deseados a comparar, y el año que se desea analizar

Por último en la entrada 13 tenemos la creacion del grafico:
- Primer argumento es el indicador que compararemos entre los paises
- Segundo argumento pasaremos la lista de los paises que creamos en el punto anterior
- El tercer argumento representa el año que indicamos también en la entrada anterior
- Cuarto argumento el tipo de índice a medir (porcentaje o numerico)
- El último argumento será el nombre del gráfico

Con esto, podremos crear cualquier tipo de información que necesitemos, si queremos indagar en índices que no se encuentre en sistema, podremos modificar la entrada, especificamente la línea:
#print(df_clean['Indicator Name'])

en el cual se puede eliminar el primer símbolo de gato (#) para mostrar todos los índices existentes (se recomienda revisar la configuración de la libreria pandas para evitar un excesivo numero de lineas)


Resultados:

Se analizó directamente el pais "Chile" en sus estadísticas. 

Se puede apreciar, a modo de conocimiento, un lento incremento de la cantidad de mujeres en relación a los hombres, debido a que el índice es prácticamente 50/50 en el nacimiento, se puede inferir que existen otros factores que expliquen un aumento en la relacion en cantidad de mujeres por sobre los hombres (por ejemplo la mortalidad).

Luego nos encontramos con la probabilidad de llegar a los 65 años de vida, por la causa que sea. Si bien se ve una gran mejora en la calidad de vida y extensión en los años (debido probablemente a mayor esperanza de vida por una mejor salud y tecnologia), la probabilidad de llegar a los 65 años es bastante elevada, pero sigue siendo mayor en las mujeres (tambien explicando el primer grafico e indiciando una mortalidad más alta en hombres)

Para ratificar, la mortalidad a continuación nos indica una tasa que si bien va en baja en terminos generales (la cual ha ido mejorando con el tiempo), la diferencia entre hombres y mujeres sigue siendo un tema principal a analizar.

Un punto importante es como a partir del 2020 (fecha en que empieza la pandemia) la tasa de mortalidad (probablemente por producto del Covid) ha ido en aumento.

Debido también a la baja general en mortalidad y esperanza de vida, se puede observar como la población mayor a los 65 años ha ido en aumento, estando muy cerca de igualar a la sociedad jóven (menor a 15 años), la cual por términos también de natalidad ha ido bajando y el porcentaje de personas entre 15-65 años fue reforzada.

Un punto importante es la tasa de mortalidad de infantes hombres, nuevamente si bien gracias a la salud ha mejorado a nivel global, de manera significativa, siempre la mortalidad infantil ha estado superior en hombres.

La tasa de fertilidad por mujer también ha decaido demasiado (cosa que también explica que la población Juvenil esté en decadencia) y la población mayor a 15 años esté en aumento, mientras siga la esperanza de vida creciendo tendremos más personas por sobre los 65 años

Y finalmente tenemos el ratio entre la gente dependiente por edad. Nuevamente a términos generales ha ido disminuyendo la gente la cual es dependiente (de personas entre 15-65 dependientes), se observa como la juventud pasó de tener una dependencia muy alta a ir disminuyendo mucho más, a esto le podemos atribuir muchas causas, trabajo juvenil sobre todo, o estadísticas delictuales, y como al aumentar la esperanza de vida y al tener personas por sobre los 65 años, hay mayor cantidad de personas por sobre los 65 que requieren de otra para vivir. 


Alcance de la información:

Si bien se analizaron puntos muy específicos para ésta investigación, tenemos una amplia gama de tablas que se pueden crear, generar comparativas entre distintos países, pudiendo ser usado por cualquier persona incluso
sin necesidad de conocer a cabalidad la programación usada.

También, si se necesitara, se pueden acceder a muchos más índices que los mostrados, ya que solamente se establecieron los más completos y llamativos, pero gracias a los filtros establecidos, podemos revisar fácilmente 
todos los indicadores que existen en el dataframe.

