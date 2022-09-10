# Modelo de IA con uso de Librerias

Utilizando la base de datos 'wine', se implementara un modelo de regresión logística aprovechando la libreria de sklearn. Este conjunto de datos consiste en el análisis químico de diferentes vinos cosechados en la mima region de Italia, pero en diferentes viñedos. El análisis cuenta con 13 variables encontradas en los tres tipos de vinos.


Las variables son:

1) Alcohol 
2) Malic acid: Acido málico
3) Ash: Ceniza 
4) Alcalinity of ash: Alcalinidad de la ceniza
5) Magnesium: Magnesio
6) Total phenols: Total de fenoles
7) Flavanoids: Flavonoides
8) Nonflavanoid phenols: Fenoles no flavonoides 
9) Proanthocyanins: Proantocianidina
10) Color intensity: Intensidad del color 
11) Hue: Matiz 
12) OD280/OD315 of diluted wines: OD280/OD315 diluido en el vino
13) Proline: Prolina

La regresion logística fue variando el numero de iteraciones utilizando 5, 15, 50, 1000 y 10000 iteraciones. Al utilizar la metrica de precision, se puede ver que hay una mejora, sin embargo, no es tan significativa despues de las 50 iteraciones. 

Los resultados obtenidos fueron los siguientes: 

- Score 52.54237288135594 % con 5 iteraciones
- Score 69.49152542372882 % con 15 iteraciones
- Score 96.61016949152543 % con 50 iteraciones
- Score 98.30508474576271 % con 1000 iteraciones
- Score 100.0 % con 10000 iteraciones

Utilizando el último modelo, podemos ver que este tiene una precision del 100%. Por lo que en las demas metricas como f1, precision y exhaustividad tienen una calificacion de 1. Finalmente, al graficar las probabilidades del modelo, podemos ver que este tienen un sesgo bajo, con los datos distribuidos de manera similar, una varianza media, con un rango amplio, mas no exagerado en la seleccion de los datos y tiene overfitting, ya que la precisión es muy alta y se ajusta perfectamente a los datos. 
