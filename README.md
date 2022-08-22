
# Parcial 1

## 1) ¿Qué tipo de variables tiene el dataset? Detalle el tipo de variable de cada columna.

|Campo|Tipo|
|-|-|
|gender| Categorica nominal|
|race/ethnicity| Categorica nominal|
|parental level of education| Categorica ordinal |
|lunch| Categorica nominal|
|test preparation course | Categorica nominal|
|math score | Cuantitativa|
|reading score | Cuantitativa|
|writing score | Cuantitativa |

## 2) ¿Qué tipo de problemas de calidad de datos logra identificar? Defina e implemente las estrategias de limpieza de datos que correspondan.

1) Todos los campos presentan perdida de datos, es decir en todos los casos hay datos faltantes (nan), para corregirlo se hizo lo siguiente:

- En todas las variables categoricas se agrego una nueva categoria llamada "not reported"
- En las variables cuantitativa se reemplazaron los valores por la media de toda la columna

2) En la variable ***parental level of education*** se presentaban valores unicos que definian lo mismo por lo que se hizo lo siguiente:

- ***some high school*** se reemplazo por ***high school*** 
- ***some college*** se reemplazo por ***bachelor's degree***

## 3) ¿En qué asignatura en promedio los estudiantes obtuvieron un mejor puntaje?
La asignatura con mayor promedio fue "reading score":
|Materia| Promedio|
|-|-:|
|math score | 66.12|
|reading score | 69.257|
|writing score | 68.18|

![Alt text](https://i.imgur.com/S4bRRfI.png)
### 3.1 ¿Hay evidencia de algún sesgo en la distribución de dichos puntajes?
Hay 2  casos de posibles sesgos en la distribución de puntajes:

Aparentemente los estudiantes con padres con un nivel de maestria obtienen mejores promedios en todas las materias
![Alt text](https://i.imgur.com/aKBuVjK.png )

En cuanto a raza, los estudiantes del grupo E tienen mejores promedios que los demas, denotando posible sesgo etnico.
![Alt text](https://i.imgur.com/sIJ9XIS.png )

## 4) ¿Existe alguna correlación entre los puntajes obtenidos en las tres asignaturas?

| |math score| reading score |	writing score |
|-|-:|-:|-:|	
|math score |	1.000000 |	0.780656 |	0.752299|
|reading score |	0.780656 |	1.000000 |	0.909290|
|writing score |	0.752299 |	0.909290 |	1.000000|

Existen altas correlaciones entre las materias, todas por encima de 0.7, siendo la mayor la correlacion entre ***math score*** y ***reading score*** con un valor de 0.9.
Esto indica que hay cierta nivelacion entre las notas, es decir, los estudiantes mantienen un promedio similar en todas las materias.

## 5) ¿Hay alguna diferencia observable en los puntajes de la asignatura de matemáticas entre géneros? ¿Qué género obtuvo en promedio los mejores puntajes?

El genero con mayor puntaje es el masculino con 68.52, los promedios estan muy cercanos entre generos.
|Genero | Promedio Math|
|-|-:|
|female| 63.583491|
|male | 68.522383 |
|non-binary | 67.706014|
|not reported | 64.449362 |

## 6) ¿Qué nivel de escolaridad tienen los padres de los estudiantes que obtuvieron un puntaje por encima del percentil 85 en la asignatura de escritura? ¿Cómo se distribuye la escolaridad entre esta población?

	
|parental level of education |	cantidad |	PORCENTAJE|
|-|-:|-:|	
|associate's degree	| 36|	24.66 % |
|bachelor's degree |	57 |	39.04 % |
|high school |	25 |	17.12 % |
|master's degree |	19 |	13.01 % |
|not reported |	9 |	6.16 %|

![Alt text](https://i.imgur.com/qFD3VWf.png)

El mayor grupo es el de padres con un nivel universitario.

## 7) ¿Qué porcentaje de los estudiantes obtuvieron puntajes iguales o superiores a 90 en las tres asignaturas? 

En total solo **19** estudiantes superaron el puntaje de 90 en las 3 materias.

### 7.1 De estos estudiantes¿que porcentaje estudió para los exámenes?

Un 52.63% de estos estudiantes se prepararon para el examen, un 42.1% no lo hicieron lo que indica que no necesariamente la preparacion fue la razon por la que obtuvieron un puntaje tan alto.
	
|test preparation course |	 cantidad |	PORCENTAJE|
|-|-:|-:|	
|completed |	10 |	52.63% |
|none |	8 |	42.10%|
|not reported |	1 |	5.26 %|

![Alt text](https://i.imgur.com/lmU8H5C.png)


# Punto 5

URL vídeo Youtube:

https://youtu.be/HM1m2UxEiqo
