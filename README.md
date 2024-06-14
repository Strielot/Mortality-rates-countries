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

Desde la entrada 7, podemos observar la lista de todos los indicadores que podemos utilizar para hacer el análisis, para usar el nombre de éstos en los gráficos que queramos.

En la entrada 9, tenemos nuestras listas de indicadores, de los cuales se armarán los gráficos, cada lista corresponde a un gráfico distintos, podemos editar los existentes o crear nuestras propias listas desde los indicadores revisados anteriormente.

Luego en la entrada 10 tenemos la creación de los gráficos, cada gráfico tendrá:
- Como primer argumento el país que se analizará.
- Segundo argumento la lista de indicadores que creamos en el punto anterior (entrada 9).
- Nuestro tercer argumento será el nombre de nuestro gráfico.
- el ultimo argumento, "numeric" o "porcentage" se refiere a si el gráfico tendrá valores numéricos o en algun porcentaje %.

En la entrada 12 tenemos nuevos parámetros a ingresar para ahora analizar distintos paises con el mismo indicador. Se deberán ingresar en este caso dos parámetros, una lista con los paises deseados a comparar, y el año que se desea analizar

Por último en la entrada 13 tenemos la creacion del grafico:
- Primer argumento es el indicador que compararemos entre los paises.
- Segundo argumento pasaremos la lista de los paises que creamos en el punto anterior (entrada 12).
- El tercer argumento representa el año que indicamos también en la entrada anterior.
- Cuarto argumento el tipo de índice a medir (porcentaje o numerico).
- El último argumento será el nombre del gráfico.

Con esto, podremos crear cualquier tipo de gráfico que necesitemos, si queremos indagar en índices que no se encuentre en los gráficos a analizar, podremos modificar la entrada, especificamente la línea:
#print(df_clean['Indicator Name'])

en el cual se puede eliminar el primer símbolo de gato (#) para mostrar todos los índices existentes (se recomienda revisar la configuración de la libreria pandas para evitar un excesivo numero de lineas)


Resultados:

Se analizó directamente el pais "Chile" en sus estadísticas. 

En nuesrto primero gráfico se puede apreciar, un lento incremento de la cantidad de mujeres en relación a los hombres, debido a que el índice en el nacimiento es prácticamente 50/50 en el género, se puede inferir que existen otros factores que expliquen un aumento en la relacion en cantidad de mujeres por sobre los hombres (por ejemplo la mortalidad).

Luego nos encontramos con la probabilidad de llegar a los 65 años de vida, por la causa que sea. Si bien se ve una gran mejora en la calidad de vida y extensión en los años (debido probablemente a mayor esperanza de vida por una mejor salud y tecnologia), la probabilidad de llegar a los 65 años es bastante elevada, pero sigue siendo mayor en las mujeres (tambien explicando el primer grafico e indiciando una mortalidad más alta en hombres)

Para ratificar, la mortalidad nos indica una tasa que si bien va en baja en terminos generales (la cual ha ido mejorando con el tiempo), la diferencia entre hombres y mujeres sigue siendo un tema principal.

Un punto importante es como a partir del 2020 (fecha en que empieza la pandemia) la tasa de mortalidad (probablemente por producto del Covid) ha ido en aumento.

Debido también a la baja general en mortalidad y esperanza de vida, se puede observar como la población mayor a los 65 años ha ido en aumento, estando muy cerca de igualar a la sociedad jóven (menor a 15 años), la cual por términos también de natalidad ha ido bajando y el porcentaje de personas entre 15-65 años fue reforzada.

Un punto importante es la tasa de mortalidad de infantes hombres, nuevamente si bien gracias a la salud ha mejorado a nivel global, de manera significativa, siempre la mortalidad infantil ha estado superior en hombres.

La tasa de fertilidad por mujer también ha decaido demasiado (cosa que también explica que la población Juvenil esté en decadencia y la población mayor a 15 años esté en aumento), mientras siga la esperanza de vida creciendo tendremos más personas por sobre los 65 años.

Y finalmente tenemos el ratio entre la gente dependiente por edad. Nuevamente a términos generales ha ido disminuyendo la gente la cual es dependiente (de personas entre 15-65 dependientes), se observa como la juventud pasó de tener una dependencia muy alta a ir disminuyendo mucho más, a esto le podemos atribuir muchas causas, trabajo juvenil sobre todo, o estadísticas delictuales, y como al aumentar la esperanza de vida y al tener personas por sobre los 65 años, hay mayor cantidad de personas por sobre los 65 que requieren de otra para vivir. 


Alcance de la información:

Si bien se analizaron puntos muy específicos para ésta investigación, tenemos una amplia gama de tablas que se pueden crear, generar comparativas entre distintos países, pudiendo ser usado por cualquier persona incluso
sin necesidad de conocer a cabalidad la programación usada.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

English:

Introduction:

One of the maing challenges in a country, is to control the population and establish campaigns to improve people's quality of life. The statistics that will be reviewed rely on the study of the national populatio, spsecifics to birth and mortality rates, to understand the current state of the country, identify inflection points, events that might cause these inflections, and above all, find solutions to problems that will be reflected in future numbers.

Within the information, we can divide the development into two major branches:

a) Progressive analysis of the country, considering the development of an indicator over time, its progression through history, and events that might influence the change.

b) A comparison of the statistics with other countries to understand the differences and the possible improvements that can be adopted from countries with better statistics.


Where can these data be found?

These data are publicly available at https://data.worldbank.org/.

They were specifically extracted from https://www.kaggle.com/datasets/programmerrdai/global-life-expectancy-at-birth/data, which is a compilation of the information.


Method of Use:

From entry 7, we can see the list of all indicators that we can use for analysis, to create lists using their names so we can create the charts we need.

In entry 9, we have our lists of indicators, from which the charts will be made. Each list corresponds to a different chart, and we can edit them or create our own lists from the previously reviewed indicators.

Then in entry 10, we have the creation of the charts. Each chart will have:

- The first argument is the country to be analyzed.
- The second argument is the list of indicators we created in the previous step (entry 9).
- The third argument will be the name of our chart.
- The last argument, "numeric" or "percentage," refers to whether the chart will have numerical values or it will represent a percentage % of the total.

In entry 12, we have new parameters for input to analyze different countries with the same indicator. In this case, two parameters must be entered: a list of the desired countries to compare, and the year to be analyzed.

Finally, in entry 13, we have the creation of the chart:

- The first argument is the indicator we will compare between countries.
- The second argument is the list of countries we created in the previous step (entry 12).
- The third argument represents the year we indicated in the previous entry.
- The fourth argument is the type of index to measure (percentage or numeric).
- The last argument will be the name of the chart.
  
With this, we can create any type of chart we need. If we want to explore indices that are not in this analysis, we can modify the entry, specifically the line:

#print(df_clean['Indicator Name'])
In which the first hash symbol (#) can be removed to display all existing indices (it is recommended to check the pandas library configuration to avoid an excessive number of lines).

Results:

*Only the statistics of the country "Chile" were analyzed.*

In our first chart, it can be noted a slow increase in the number of women relative to men. Since the birth ratio is practically 50/50 for gender, it can be inferred that there are other factors explaining an increase in the number of women compared to men (e.g., mortality).

Next, we have the probability of reaching the age of 65, regardless of the cause. Although there is a significant improvement in quality of life and life expectancy (probably due to better health and technology), the probability of reaching 65 years is quite high but still higher for women (also explaining the first chart and indicating higher mortality in men).

And to confirm, the mortality rate indicates a rate that, although generally decreasing (which has improved over time), the difference between men and women remains a key issue.

An important point to note now, is how starting from 2020 (the onset of the pandemic), the mortality rate (probably due to COVID) has been increasing.

Due also to the general decline in mortality and increased life expectancy, it can be observed that the population over 65 years old has been increasing, coming very close to matching the young population (under 15 years old), which has been declining (due to a lower birth rate), and the percentage of people between 15-65 years has been reinforced.

An important point is the male infant mortality rate, which, although improved significantly globally due to better health, has always been higher for males.

The fertility rate per woman has also significantly declined (which also explains the declining young population, and the population over 15 years old is increasing). As long as life expectancy continues to grow, we will have more people over 65 years old.

Finally, we have the ratio of dependent people by age. Again, in general terms, the number of independent people (people between 15-65 years) has been decreasing. It is observed how the youth went from having a very high dependency to decreasing much more. This can be attributed to many causes, especially youth employment or crime statistics. As life expectancy increases and there are more people over 65 years old, there is a greater number of people over 65 who require assistance to live.


Scope of the Information:

While very specific points were analyzed for this research, we have a wide range of tables that can be created, generating comparisons between different countries, which can be used by anyone even without fully understanding the programming used.

Additionally, if needed, many more indices can be accessed beyond those shown, as only the most comprehensive and interesting ones were established. However, thanks to the established filters, we can easily review all the indicators that exist in the dataframe.
