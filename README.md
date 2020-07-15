# Practica5
Informe #5
# *TEOREMA DE SUPERPOSICIÓN*
## *PLANTEAMIENTO DEL PROBLEMA*
Se han observado diferentes técnicas para la resolución de circuitos, entre ellos el análisis nodal y el análisis de mallas, todo esto bajo la aplicación de las Leyes de Kircchoff y la Ley de Ohm. Pero cuando en un circuito encontramos más de dos fuentes de voltajes, ya sea de corriente, de voltaje o ambas, el cálculo de voltaje o corriente en cada uno de sus componentes resulta ser mucho más complicado. Es por esto que surge una nueva técnica, el teorema de la Superposición, del cual queremos conocer que tan efectivo es y para esto también tendremos que comprobarlo.

## *OBJETIVOS:*
# Objetivo general
- Diseñar un circuito electrico mediante la simulación en laboratorios virtuales para comprobar el teorema de Superposición.

# Objetivos específico
- Comprender la metodología de la Superposición para clarificar los conceptos previamente adquiridos en la teoría.
- Comparar los resultados teóricos con los prácticos para encontrar el error entre mediciones obtenidas.



## *LISTA DE MATERIALES:*


| Cantidad | Material de Equipo |
| ------------- | ------------- |
| 2  | Fuente de voltaje de C.D. |
| 2  | Multímetros digitales |
|  1 | Resistor de 1k  |
|  1 | Resistor de 2.2k  |
|  1 | Resistor de 820k  |
|  1 | Resistor de 470k  |
| 1  | Protoboard      |

## *MARCO TEÓRICO*
El teorema de la superposicion se puede utilizar tanto en AC como en DC , para poder determinar si se puede aplicar este método debemos tomar en cuenta que solo es aplicable para circuitos lineales , que estan conformados por componentes en las cuales la corriente es directamente proporcional a la tensión de sus terminales.

Este método nos ayuda a calcular tanto como voltajes , intensidades en las cuales halla varias fuentes de energía (fuentes de voltaje, fuentes de corrientes) y para obtener el resultado de este procedimiento se puede hallar sumando la tensión del circuito a cada una de las fuentes (independientes) por separado.

![alt text](https://github.com/Kevi7k/Practica4/blob/master/Img/Fig1.png)

Fig 1. Superposición

Los pasos a seguir son los siguientes:

1) Se quitan las todas las fuentes excepto una, tomar en cuenta que si anulamos un voltaje este se convierte en corto circuito y si anulamos una corriente se hace un circuito abierto

![alt text](https://github.com/Kevi7k/Practica4/blob/master/Img/Voltaje%20apagado.png)

Fig 2. Voltaje transformado

![alt text](https://github.com/Kevi7k/Practica4/blob/master/Img/Corriente%20apagada.png)

Fig 3. Corriente transformada


2) Se calcula el voltaje y intensidades solo con la fuente que no se quito.

3) Se repiten los pasos 1 y 2 con cada fuente.

4) Se suman las respuestas de cada fuente (Tomar en cuenta los signos con lo que se desplaza la corriente , en algunos casos puede restarse)


## *PROCEDIMIENTO*
1. Implemente el siguiente circuito que se muestra en la figura:

![alt text](https://github.com/Kevi7k/Practica4/blob/master/Img/Diagrama%201.jpg)

Fig.4. Circuito para comprobar el teorema de Superposición

2. Con las dos fuentes conectadas, mida el voltaje VA y la corriente IX, respetando tanto la polaridad del voltaje como el sentido de la corriente que se proporcionan. Anote el valor de las mediciones en la tabla 4.1 y 4.2 respectivamente.

3. Haga “cero” la fuente de voltaje de 12 V (V2) y mida el voltaje VA y la corriente IX, respetando tanto la polaridad del voltaje como el sentido de la corriente que se proporcionan. Anote el valor de las mediciones en la tabla 4.1 y 4.2 respectivamente.

4. Haga “cero” la fuente de voltaje de 20 V (V1) y mida el voltaje VA y la corriente IX, respetando tanto la polaridad del voltaje como el sentido de la corriente que se proporcionan. Anote el valor de las mediciones en la tabla 4.1 y 4.2 respectivamente.

## *TABULACIÓN DE DATOS*

|Tipo de dato|Voltaje Total (Va)| Voltaje (Va)cuando V2=0 |Voltaje (Va)cuando V1=0|
| ------------- | ------------- | ------------- | ------------- |
| Calculado | 959[mV] | 7,479[V] | 6,52[V] |
| Medido | 952[mV] | 7,48[V] | 6,53[V] |

TABLA I. Medición de voltaje aplicando superposición

|Tipo de dato|Corriente Total (Ix)| Corriente (Ix) cuando V2=0 |Corriente (Ix) cuando V1=0|
| ------------- | ------------- | ------------- | ------------- |
| Calculado | 25,51[mA] | 0[A] | 25,51[mA] |
| Medido | 25,5[mA] | 0[A] | 25,5[mA] |

TABLA II. Medición de corriente aplicando superposición

## *DIAGRAMA*

![alt text](https://github.com/Kevi7k/Practica4/blob/master/Img/Diagrama%205.jpeg)

Fig.5. Circuito Simulado en DCAClab

![alt text](https://github.com/Kevi7k/Practica4/blob/master/Img/Diagrama%206.jpg)

Fig.6. Circuito Simulado en TinkerCAD

## *Ecuaciones*

Las ecuaciones que vamos a utilizar para este tema, prácticamente son las mismas de temas anteriores.Lo único que cambia es la metodología al momento de resolver, como los pasos a seguir que tenemos en el marco teórico:

Ley de Ohm I=V/R

Intensidad=Amperio (A)

Voltaje=Voltio (V)

Resistencia= Ohmio (omega)

Una vez obtenido este modelo matemático podemos afirmar que se cumple la siguiente ley:

V1+V2+V3+V4+...Vn=0

Esta ecuación se cumple siempre y cuando sea de solamente una malla, es decir la sumatoria de voltajes dentro de una malla es igual a cero, afirmando eso se cumple otra ley que nos habla sobres las corrientes:

I(salida)=I(entrada)


## *EXPLICACIÓN DEL CIRCUITO*

En nuestro circuito podemos evidenciar, dos fuentes de voltaje, de 20 V y de 12 V, que serán las que suministren energía al sistema. También contaremos con 4 resistencias, de 1000, 2200, 820 y 470 ohmios. Conectados dichos elementos como podemos evidenciar en nuestros diagramas. Nuestro primer elemento será nuestra fuente de voltaje de 20 V, del polo positivo de nuestra fuente de voltaje, tendremos nuestra resistencia de 1000 ohmios, de la cual tendremos dos resistencias, es decir que nuestra corriente se dividirá en dos. Nuestra primera resistencia resultante es la de 2200 ohmios, la cual saldrá a los polos negativos de las fuentes. La otra resistencia resultante será nuestra resistencia de 820 ohmios, de la cual luego calcularemos la caída de tensión, que tomaremos como Va, y de dicha resistencia tendremos otra división de corriente, la primera es en nuestra resistencia de 470 ohmios, que terminara en los polos negativos de nuestras fuentes, la cual calcularemos el paso de corriente y lo llamaremos Ix. Y, por último, también nuestra resistencia de 820 ohmios estará conectado al polo positivo de nuestra segunda fuente de voltaje. Y los polos negativos de nuestras fuentes estarán conectados entre sí. 

Para nuestro teorema de superposición, podemos calcular los valores de Va e Ix, tomando dos casos distintos, el primer caso apagando nuestra segunda fuente y trabajando como si tuviéramos una sola fuente, y el segundo caso que será apagar nuestra primera fuente y trabajar como si solo tuviéramos una fuente. Al final, al tener nuestros resultados por separado, solo tendremos que sumar nuestros valores respectivos de Va e Ix y tendremos nuestros valores que estamos buscando.


## *ANÁLISIS DE RESULTADOS*
En general los resultados de las mediciones nunca serán exactas, a pesar del máximo cuidado que se tenga en el momento de realizar cada una de ellas, no es posible expresar el reultado como exacto, es por esto que a continuación se ralizará una tabla donde se muestre  el error relativo de cada valor obtenido:

|Voltaje (Va)| Resultados Analíticos |Resultados Experimentales|%Error|
| ------------- | ------------- | ------------- | ------------- |
| Cuando V2=0 | 7,479 [V] | 7,48 [V] | 0,013%|
| Cuando V1=0 | 6,52 [V] | 6,53 [V] | 0,153% |
| Voltaje total |959[mV] | 952 [mV] | 0,73% |

TABLA III. Cálculo de errores en mediciones de voltaje

|Corriente (Ix)| Resultados Analíticos |Resultados Experimentales|%Error|
| ------------- | ------------- | ------------- | ------------- |
| Cuando V2=0 |  0[A] | 0 [A] | 0 %|
| Cuando V1=0 |25,52[mA] | 25,5 [mA] | 0,078 % |
|Corriente total | 25,52[mA]| 25,5 [mA] | 0,078 % |

TABLA IV. Cálculo de errores en mediciones de corriente

Luego de observar los resultados de analíticos y experimentales en la Tabla III. como en la Tabla IV. respecto al comportamiento de voltajes y corrientes en los elementos del circuito, que se obtienen de apagar cada una de las fuentes, se puede decir que los errores obtenidos son evidentemente valores pequeños. Lo que nos garantiza la correcta realización de los cálculos respecto a superposición.

## *CONCLUSIONES*

- A través de la comparación de los resultados obtenidos en la simulación y en los cálculos donde, al realizar la suma algebraica de cada una de las fuentes actuando por sí solas, se comprobó experimentalmente que en el circuito propuesto se cumple con el Teorema de Superposición.

- Frente a la mediciones obtenidas en el laboratorio se obtuvieron ciertos errores como se puede visualizar en la Tabla III, el valor del error relativo porcentual de Va cuando V2=0 y cuando V1=0 son 0,013% y 0,153% respectivamente, mientras que el error del Voltaje total en "a" es 0,73%, valores sumamente pequeños considerados aceptables.

- Respecto a la corriente Ix cuando V2=0 y v1=0, los errores obtenidos fueron de 0% y 0,078%. Y refiriéndonos a la corriente total Ix se obtuvo un error de 0,078%, sin embargo las mediciones obtenidas se aproximan mucho a los resultado que se calculó, por lo que consideramos a estos errores como insignificantes.

- El Teorema de Superposición nos ha resultado una técnica muy práctica de utilizar cuando tenemos varias fuentes de voltaje y corriente en un mismo circuito, ya que nos simplifica los cálculos al considerar las fuentes de voltaje como corto circuitos y las fuentes de corriente como circuitos abiertos.


## *RECOMENDACIONES*
- Se debe tomar en cuenta que cuando simulemos un circuito en el laboratorio virtual, tenemos que apagar la fuente de voltaje, más no asignarle el valor de "cero", ya que nuestros resultados pueden variar notablemente, lo que provocaría un error extremadamente grande.

- Al tener bien definido el concepto de superposición y los conceptos de las leyes más básicas, se nos facilitará realizar con mejor autonomía la práctica e identificar los errores de por medio que se pueden presentar.

- Es necesario verificar los valores que asignamos a las fuentes de voltaje como a resistencias, ya que se suele cometer errores con las unidades de medida, de igual forma que la conexión esté bien hecha para que las mediciones sean lo más exactas posibles.

- Para la obtención de medidas de corrientes y voltajes, debemos realizar bien la conexión de nuestro multímetro, es decir, ser estricto en cuanto a la conexión del positivo y negativo ya que si no lo colocamos bien, probablemente obtengamos resultados diferentes a los solicitados, que pueden afectar a cálculos secundarios.


## *CRONOGRAMA*

![alt text](https://github.com/Kevi7k/Practica4/blob/master/Cronograma/Cronograma_Pr%C3%A1ctica4.jpg)

## *BIBLIOGRAFÍA*

Charles K. Alexander, Matthew N. O. Sadiku, Fundamentos de circuitos eléctricos. Tercera edición. México: McGrawHill, 2004.

## *ANEXOS*

![alt text](https://github.com/Kevi7k/Practica4/blob/master/Img/Medicion%201.jpeg)

Fig. 7. Mediciones(V2=0)

![alt text](https://github.com/Kevi7k/Practica4/blob/master/Img/Medicion%202.jpeg)

Fig. 8. Mediciones(V1=0)

![alt text](https://github.com/Kevi7k/Practica4/blob/master/Img/Medicion%203.jpeg)

Fig. 9. Mediciones 

![alt text](https://github.com/Kevi7k/Practica4/blob/master/Img/Resolucion%20ejercicio.jpeg)

Fig. 10. Resolución del ejercicio

![alt text](https://github.com/Kevi7k/Practica4/blob/master/Img/Calculo%20de%20errores.jpeg)

Fig. 11. Cálculo de los errores. 
