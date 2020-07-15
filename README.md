# Práctica 5
# *TEOREMA DE THÉVENIN*
## *PLANTEAMIENTO DEL PROBLEMA*
A lo largo de la asignatura, se han visto una variedad de métodos para la resolución de circuitos eléctricos, sin embargo es frecuente encontrarnos con circuitos realmente complejos, los cuales suelen ser muy complicados resolver con las técnicas aprendidas anteriormente, es por esta razón que surge la necesidad de comprender el teorema de Thévenin, que resume un circuito, cualquiera que sea, en un circuito básico con un resistencia y un voltaje. Antes de hacer uso de este método será necesario validar este teorema a través de la práctica mediante su respectiva comprobación experimental.
## *OBJETIVOS:*
# Objetivo general
- Diseñar un circuito electrico mediante la simulación en laboratorios virtuales para comprobar la validez del teorema de Thévenin

# Objetivos específico
- Comprender la metodología del teorema de Thévenin para reafirmar los conocimientos previamente adquiridos.
- Analizar los resultados teóricos con los prácticos mediante la comparación de los mismos para la obtención de porcentajes de error respectivos.


## *LISTA DE MATERIALES:*


| Cantidad | Material de Equipo |
| ------------- | ------------- |
| 2  | Fuente de voltaje de C.D. |
| 2  | Multímetros digitales |
|  1 | Resistor de 560  |
|  1 | Resistor de 4.7k  |
|  1 | Resistor de 330  |
|  1 | Resistor de 100 |
|  1 | Resistor de 1k  |
|  1 | Potenciómetro de precisión de 1k|
|  1 | Protoboard      |

## *MARCO TEÓRICO*
El teorema de Thévenin nos dice  que cualquier red de corriente lineal de dos terminales puede ser reemplazada por un circuito equivalente que contiene un voltaje y una resistencia equivalente en serie.

Entonces tenemos que si una resistencia está enlazada a un circuito entre los puntos A y B y reemplazamos el circuito por el otro equivalente entonces en la resistencia va a recorrer la misma intensidad.

![alt text](https://github.com/Kevi7k/Practica5/blob/master/Im%C3%A1genes/Diagrama%201.png)

Figura 1. Diagrama del teorema de Thévenin

El valor de la fuente del circuito resultante se denomina tensión de Thévenin y se consigue resolviendo la tensión del circuito entre A y B sin tomar en cuenta la resistencia entonces lo que produce esto es un circuito abierto.

Entonces, ahora el valor de la resistencia resultante  en serie se denomina resistencia de Thévenin y se calcula como si existiera una resistencia en los puntos A y B sin tomar en cuenta el valor de la resistencia y poniendo en cortocircuito a todas las fuentes de voltaje

![alt text](https://github.com/Kevi7k/Practica5/blob/master/Im%C3%A1genes/Diagrama%202.png)

Figura 2. Ejemplo del teorema de Thévenin



## *PROCEDIMIENTO*
1. Prepare el laboratorio virtual de su preferencia y arme el circuito que se muestra en la figura

![alt text](https://github.com/Kevi7k/Practica5/blob/master/Im%C3%A1genes/Diagrama%203.png)

Figura 3.  Circuito para comprobar el Teorema de Thévenin.
  
2. Con el circuito sin ningún tipo de modificación, mida el voltaje y la corriente en el resistor R5, anote los resultados en la tabla 5.2.

3. Desconecte el resistor R5 y mida el voltaje en el circuito abierto. Anote el valor
medido en la tabla.

4. Anule el efecto de las fuentes de alimentación. Desconecte R5 y desde el circuito
abierto resultante mida la resistencia equivalente. Anote el valor medido en la tabla.

5. Implemente el circuito equivalente de Thévenin, agregue el resistor R5 y mida la
corriente y el voltaje en el mismo, anote los resultados en la tabla.


## *TABULACIÓN DE DATOS*

|Tipo de dato |VTH (V) |RTH (Ω)| 
| ------------- | ------------- | ------------- | 
| Calculado     | 5.056     |  298.8558    | 
| Medido     | 5.06         |      299    |    


TABLA I. Valores del Circuito Equivalente de Thévenin

|                      |  Circuito | Original |  Circuito | Thévenin |
|:--------------------:|:---------:|:--------:|:---------:|:--------:|
| Parámetro  eléctrico | Calculado |  Medido  | Calculado |  Medido  |
|      Voltaje (V)     |   3.8926  |   3.89   |   5.056   |   5.06   |
|    Corriente (mA)    |   3.8926  |   3.89   |  15.3212  |   15.3   |

TABLA II. Comprobación del Teorema de Thévenin

## *DIAGRAMA*

![alt text](https://github.com/Kevi7k/Practica5/blob/master/Im%C3%A1genes/Circuito_Original.png)

Figura 3. Circuito propuesto simulado en TinkerCAD.

![alt text](https://github.com/Kevi7k/Practica5/blob/master/Im%C3%A1genes/Circuito_Thevening.png)

Figura 4. Implementación del circuito de Thévenin.

## *Ecuaciones*

Las ecuaciones que vamos a utilizar para este tema, prácticamente son las mismas de temas anteriores.Lo único que cambia es la metodología al momento de resolver, como los pasos a seguir que tenemos en el marco teórico pero tomando en cuenta lo siguiente:

La resistencia de Thévenin es la resultante de todas las resistencia en el circuito pero apagado las fuentes y se denomina como (Rth)

El voltaje de Thévenin esta denominado con (Vth):

Vth=In.Rth

Donde In vendría ser la intensidad de donde quitamos la resistencia , cumpliendose Ley de Ohm y las unidades son las mismas.

Intensidad=Amperio (A)

Voltaje=Voltio (V)

Resistencia= Ohmio (omega)

Para encontrar las corrientes necesarias para el calculo de voltajes, tanto en el circuito original como en el circuito de Thévenin será necesario hacer uso de las leyes de Kirchoff. De manera que:

V1+V2+V3+V4+...Vn=0

Esta ecuación se cumple siempre y cuando sea de solamente una malla, es decir la sumatoria de voltajes dentro de una malla es igual a cero, afirmando esto, se cumple otra ley que nos habla sobres las corrientes. Es muy útil si para el cálculo realizaramos un análisis nodal

I(salida)=I(entrada)


## *EXPLICACIÓN DEL CIRCUITO*

Para nuestra práctica, tenemos un circuito el cual está conformado por dos fuentes de voltaje, y 5 resistencias. Los valores de las fuentes de voltaje son de 12 V y de 2V, las resistencias son de 560, 4700, 330, 100 y 1000 ohmios, esta última será tomada como nuestra resistencia que la vamos a excluir para sacar nuestra resistencia y nuestro voltaje Thevenin. La corriente desde nuestra fuente de voltaje de 12 V, hasta nuestra resistencia de 560 ohmios. De esta resistencia saldrá una resistencia de 4700 ohmios, la cual se conectara su otro extremo con el polo negativo de la primera fuente, Y también de la resistencia de 560 ohmios, estará conectado con el polo negativo de la segunda fuente de voltaje que es de 2 V. Des nuestra segunda fuente de voltaje, saldrán dos resistencias, la primera que será de 330 ohmios y que se conectara con el polo negativo de nuestra primera fuente de voltaje, y la segunda resistencia que es de 100 ohmios, que estará conectada en serie con nuestra resistencia de 1000 ohmios, la cual terminara en el polo negativo de nuestra primera fuente de voltaje.

Para realizar nuestros voltajes en Thevenin vamos a realizar lo siguiente. Para nuestra resistencia en Thevenin, excluimos la resistencia de 1000 ohmios, dejando el sistema abierto en ese punto, y convirtiendo las fuentes de voltaje en cortocircuitos. Sacamos una resistencia equivalente y esta será nuestra resistencia Thevenin. Para nuestro voltaje Thevenin conectaremos las fuentes de voltaje, y conservaremos nuestra resistencia de 1000 ohmios abierto, realizamos el análisis como tenemos en anexos, y ya tendremos nuestro voltaje en thevenin.



## *ANÁLISIS DE RESULTADOS*
En general los resultados de las mediciones nunca serán exactas, a pesar del máximo cuidado que se tenga en el momento de realizar cada una de ellas, no es posible expresar el reultado como exacto, es por esto que a continuación se ralizará una tabla donde se muestre  el error relativo de cada valor obtenido:

|Voltaje (VTh)| Resultados Analíticos |Resultados Experimentales|%Error|
| ------------- | ------------- | ------------- | ------------- |
| Circuito Original | 3.8926 [V] | 3.89 [V] | 0,067%|
| Circuito equivalente de Thévenin | 5.056 [V] | 5.06 [V] | 0,0001% |

TABLA III. Cálculo de errores en mediciones de voltaje

|Corriente (Ix)| Resultados Analíticos |Resultados Experimentales|%Error|
| ------------- | ------------- | ------------- | ------------- |
| Circuito Original |  3.8926 [mA] | 3.89 [mA] | 0.067 %|
| Circuito equivalente de Thévenin |15.3212 [mA] | 15.3 [mA] | 0,0014 % |

TABLA IV. Cálculo de errores en mediciones de corriente

|Resistencia (Ω)| Resultados Analíticos |Resultados Experimentales|%Error|
| ------------- | ------------- | ------------- | ------------- |
| Circuito Thévenin |  298.8552[Ω] | 299 [Ω] | 0.048 %|


TABLA V. Cálculo de errores en las resistencias.



## *CONCLUSIONES*

- Se ha comprobado y validado la efectividad del teorema de Thévenin, ya que al realizar una comparación entre los datos teóricos arrojados por el método y las mediciones realizadas en el laboratorio virtual llegamos a los mismos resultados, con sus respectivas variaciones respecto al error.

- Los errores obtenidos son relativamente pequeños, de manera que su insignificancia nos conduce a afirmar que la práctica se realizó de una forma correcta. Los errores obtenidos surgen ya sea por la aproximaciones en los valores teóricos, por fallo humano en la medición o sensibilidad del instrumento.

- El error cometido en medir el Voltaje de Thévenin en el circuito original es de 0,067% y en el equivalente de Thévenin 0,0014% por lo que se considera que el error en estas mediciones pueden ser despreciables.

- En los cálculos sobre la resistencia de Thévenin se obtuvo un error de 0,048% esto se debe que al momento de calcular se aproximaron los decimales. 

- Realizando una comparación entre los datos calculados y medidos del circuito, tanto en corriente como en voltaje se obtiene un error relativo porcentual muy pequeño, en ambos 0.067%, error que no repercute posteriormente, por tanto se considera que su valor es ínfimose puede decir que es un error despreciables.

## *RECOMENDACIONES*

- Para realizar la práctica de una manera acertada, hay que tomar en cuenta bien los conceptos básicos sobre este teorema y asi no cometer errores tanto como en la simulación, como en la realizacion del ejercicio de manera teórica.

- Seguir paso a paso, de una manera ordenada el procedimiento para facilitar la simulación del circuito de forma correcta.

- Realizar los cálculos con el mayor cuidado al aproximar los números ya que si hay una equivocación en estos, el resultado teórico puede variar y eso nos puede generar un porcentaje más alto de error, que puede dejar en invalidez a nuestra práctica.

## *CRONOGRAMA*

![alt text](https://github.com/Kevi7k/Practica5/blob/master/Im%C3%A1genes/Cronograma.jpeg)

## *BIBLIOGRAFÍA*

Charles K. Alexander, Matthew N. O. Sadiku, Fundamentos de circuitos eléctricos. Tercera edición. México: McGrawHill, 2004.

## *ANEXOS*

![alt text](https://github.com/Kevi7k/Practica5/blob/master/Im%C3%A1genes/Voltaje_Corriente_Original.png)

Figura 5. Medición de voltaje y corriente en el circuito original.

![alt text](https://github.com/Kevi7k/Practica5/blob/master/Im%C3%A1genes/Voltaje_Corriente_Thevening.png)

Figura 6. Medición de voltaje y corriente en el circuito de Thévenin.

![alt text](https://github.com/Kevi7k/Practica5/blob/master/Im%C3%A1genes/Resistencia_Thevening.png)

Figura 7. Medición de resistencia en el circuito de Thévenin.

![alt text](https://github.com/Kevi7k/Practica5/blob/master/Im%C3%A1genes/Hoja_Calculos.jpg)

Figura 8. Cálculo de datos teóricos.

![alt text](https://github.com/Kevi7k/Practica5/blob/master/Im%C3%A1genes/Calculo_Error.jpeg)

Figura 9. Cálculo de errores.

