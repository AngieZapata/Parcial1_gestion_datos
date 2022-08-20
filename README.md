# Parcial1_gestion_datos
Parcial 1 para la materia de gestión de datos 


1. ¿Qué tipo de variables tiene el dataset? Detalle el tipo de variable de cada columna.

    Los tipos de variables del dataset haciendo uso de pandas con el método dtypes son: 

    gender                          object      Cualitativa (Categorica) nominal
    race/ethnicity                  object      Cualitativa (Categorica) nominal
    parental level of education     object      Cualitativa (Categorica) ordinal
    lunch                           object      Cualitativa (Categorica) nominal
    test preparation course         object      Cualitativa (Categorica) nominal
    math score                     float64      Cuantitativa continua
    reading score                  float64      Cuantitativa continua
    writing score                  float64      Cuantitativa continua


2. ¿Qué tipo de problemas de calidad de datos logra identificar? Defina e implemente las estrategias de limpieza de datos que correspondan.

    Haciendo el analisis exploratorio de datos, el unico problema que se identifica son los valores con campos nulos, para la solución se aplica dropna()


3. ¿En qué asignatura en promedio los estudiantes obtuvieron un mejor puntaje? ¿Hay evidencia de algún sesgo en la distribución de dichos puntajes?

    math score      66.26567164179104
    reading score   69.54477611940298
    writing score   68.47164179104477
    dtype: float64

    La asignatura en la que los estudiantes obtuvieron un mejor promedio fue : reading y haciendo el analisis de las graficas no se logra ver un cesgo en la distribución de los datos


4. ¿Existe alguna correlación entre los puntajes obtenidos en las tres asignaturas?

    Si, existe mayor correlación entre las asignaturas de Reading y Writing, el cual es de 0.96 y las dos anteriores con math igualmente tienen una correlación superior a 0.8


5. ¿Hay alguna diferencia observable en los puntajes de la asignatura de matemáticas entre géneros? ¿Qué género obtuvo en promedio los mejores puntajes?

        gender	    math score	reading score	writing score	promedio ponderado
    0	female	    63.647841	72.774086	    72.684385	    69.702104
    1	male	    68.383764	65.354244	    63.472325	    65.736777
    2	non-binary	68.448980	71.214286	    69.357143	    69.673469

    Haciendo los respectivos promedios, no se logra ver una gran diferencia observable en los generos para la materia de matematicas, lo unico es que el genero femenino esta 5 puntos por debajo del genero masculino y no binario. 

    El genero que obtuvo el promedio de los mejores puntajes fue el genero femenino, seguido del genero no binario


6. ¿Qué nivel de escolaridad tienen los padres de los estudiantes que obtuvieron un puntaje por encima del percentil 85 en la asignatura de escritura? ¿Cómo se distribuye la escolaridad entre esta población?.

    ['some college',
    "master's degree",
    'high school',
    'some high school',
    "associate's degree",
    "bachelor's degree"]

    Los anteriores son los grados de escolaridad de los padres para los cuales los estudiantes obtuvieron un percentil superior a 85 en escritura y la mayoria se distribuye en 'master's degree', 'associate's degree' y 'bachelor's degree'

7. ¿Qué porcentaje de los estudiantes obtuvieron puntajes iguales o superiores a 90 en las tres asignaturas? De estos estudiantes¿que porcentaje estudió para los exámenes?

    El procentaje de los estudiantes > 90 fue 5.6716417910447765% y de estos los que se prepararon paralos examenes fueron : 63.1578947368421%