# Practica5
Informe #5
# *TEOREMA DE THÉVENIN*
## *PLANTEAMIENTO DEL PROBLEMA*
............
## *OBJETIVOS:*
# Objetivo general
- Diseñar un circuito electrico mediante la simulación en laboratorios virtuales para comprobar el teorema de Thévenin

# Objetivos específico
- Comprender la metodología del teorema de Thévenin para reafirmar lo aprendido
- Comparar los resultados teóricos con los prácticos, determinando los porcentajes de errores respectivos.


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
Figura 1

El valor de la fuente del circuito resultante se denomina tensión de Thévenin y se consigue resolviendo la tensión del circuito entre A y B sin tomar en cuenta la resistencia entonces lo que produce esto es un circuito abierto.

Entonces, ahora el valor de la resistencia resultante  en serie se denomina resistencia de Thévenin y se calcula como si existiera una resistencia en los puntos A y B sin tomar en cuenta el valor de la resistencia y poniendo en cortocircuito a todas las fuentes de voltaje

![alt text](https://github.com/Kevi7k/Practica5/blob/master/Im%C3%A1genes/Diagrama%202.png)
Figura 2



## *PROCEDIMIENTO*
1. Arme el circuito que se muestra en la figura
Figura 3
  
2. Mida el voltaje y la corriente en el resistor R5, anote los resultados en la tabla 5.2.

3. Desconecte el resistor R5 y mida el voltaje en el circuito abierto. Anote el valor
medido en la tabla.

4. Anule el efecto de las fuentes de alimentación. Desconecte R5 y desde el circuito
abierto resultante mida la resistencia equivalente. Anote el valor medido en la tabla.

5. Implemente el circuito equivalente de Thévenin, agregue el resistor R5 y mida la
corriente y el voltaje en el mismo, anote los resultados en la tabla.


## *TABULACIÓN DE DATOS*

|VTH (V) |RTH (Ω)| 
| ------------- | ------------- | 
| Calculado     |  Calculado    | 
| 99(V)         |      99(Ω)    |    
|  Medido       |   Medido      |  
|  99(V)        |      99(Ω)    |

TABLA I. Valores del Circuito Equivalente de Thévenin

|Parametro electrico|  Circuito original |Circuito equivalente de Thévenin| 
| ------------- | ------------- |--------------|
| Voltaje (V) | Calculado  | Calculado |
| Voltaje (V) |  99(V)          |  99(V)   |
| Voltaje (V) | Medido        |    Medido   |
| Voltaje (V) |  99(V)          |  99(V)   |
|  Corriente(mA) | Calculado  | Calculado |
| Corriente(mA) |  99(mA)          |  99(mA)   |
| Corriente(mA) | Medido        |    Medido   |
| Corriente(mA) |  99(mA)          |  99(mA)   |

TABLA II. Comprobación del Teorema de Thévenin

## *DIAGRAMA*

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

...........

## *ANÁLISIS DE RESULTADOS*
En general los resultados de las mediciones nunca serán exactas, a pesar del máximo cuidado que se tenga en el momento de realizar cada una de ellas, no es posible expresar el reultado como exacto, es por esto que a continuación se ralizará una tabla donde se muestre  el error relativo de cada valor obtenido:

|Voltaje (VTh)| Resultados Analíticos |Resultados Experimentales|%Error|
| ------------- | ------------- | ------------- | ------------- |
| Circuito Original | 7,479 [V] | 7,48 [V] | 0,013%|
| Circuito equivalente de Thévenin | 6,52 [V] | 6,53 [V] | 0,153% |

TABLA III. Cálculo de errores en mediciones de voltaje

|Corriente (Ix)| Resultados Analíticos |Resultados Experimentales|%Error|
| ------------- | ------------- | ------------- | ------------- |
| Circuito Original |  0[A] | 0 [A] | 0 %|
| Circuito equivalente de Thévenin |25,52[mA] | 25,5 [mA] | 0,078 % |

TABLA IV. Cálculo de errores en mediciones de corriente

|Resistencia (Ω)| Resultados Analíticos |Resultados Experimentales|%Error|
| ------------- | ------------- | ------------- | ------------- |
| Circuito Original |  0[Ω] | 0 [Ω] | 0 %|
| Circuito equivalente de Thévenin |25,52[Ω] | 25,5 [Ω] | 0,078 % |

TABLA V. Cálculo de errores en las resistencias.



## *CONCLUSIONES*

-

-

-

-

## *RECOMENDACIONES*

-

-

-

-

## *CRONOGRAMA*

![alt text]

## *BIBLIOGRAFÍA*

Charles K. Alexander, Matthew N. O. Sadiku, Fundamentos de circuitos eléctricos. Tercera edición. México: McGrawHill, 2004.

## *ANEXOS*

![alt text]
