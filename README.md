# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Scarlet Angelina Ruelas Cardeña
## Grupo: B
## Fecha: 18/11/2025
## Actividad #18.  Matrices documentación


# Objetivo

El objetivo es comprender los determinantes y su importancia en la resolución de sistemas de ecuaciones, aprender técnicas como el método de Sarrus para matrices 3x3 y el cálculo de cofactores para matrices de mayor dimensión, a través de estos conceptos se busca desarrollar habilidades para analizar y resolver problemas algebraicos complejos y estudiar las propiedades fundamentales de las matrices, como la invertibilidad o su orientacion.

---
### Muestra  

*Calcula la suma de A y B*

$$
A =
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

$$
B =
\begin{pmatrix}
9 & 10 & 11 \\
12 & 13 & 14 \\
\end{pmatrix}
$$

*Desarrollo:*

$$
A + B =
\begin{pmatrix}
1 + 9 & 2 + 10 & 3 + 11 \\
4 + 12 & 5 + 13 & 6 + 14 \\
\end{pmatrix}
$$

*Resultado final:*

$$
A + B =
\begin{pmatrix}
10 & 12 & 14 \\
16 & 18 & 20 \\
\end{pmatrix}
$$

## Índice
- [Ejercicio 1: Determinantes](#ejercicio-1-clasificación-de-matrices)
- [Ejercicio 2: Metodo Sarrus y Cofactores](#ejercicio-2-operaciones-con-matrices)
- [Ejercicio 3: Aplicacion a vectores y propidades](#ejercicio-3-multiplicación-cadena)

---

# Ejercicio 1: Determinantes

## Objetivo del ejercicio: 

El objetivo es aprender a calcular y analizar los determinantes de matrices, comprender su utilidad para determinar la invertibilidad de una matriz, y aplicar estos conocimientos en la resolución de sistemas de ecuaciones lineales y en el estudio de propiedades clave, como el cálculo de áreas y volúmenes en geometría, entre otros.

### a) 
$$ A = \begin{bmatrix}
5 & 2 &\\
3 & 1 & \\
\end{bmatrix}  $$ = 
$$
\text{Det} \left( \begin{pmatrix} 5 & 2 \\ 3 & 1 \end{pmatrix} \right) = (5)(1) - (2)(3) = 5 - 6 = -1
$$
$$
\boxed{-1}
$$

### b) 
$$ B = \begin{bmatrix}
-1 & 4 & \\
2 & -8 & \\
\end{bmatrix}  $$ = 
$$
\text{Det} \left( \begin{pmatrix} -1 & 4 \\ 2 & -8 \end{pmatrix} \right) = (-1)(-8) - (4)(2) = 8 - 8 = 0
$$
$$
\boxed{0}
$$

### c)
$$ C = \begin{bmatrix}
6 & 9 & \\
2 & 3 & \\
\end{bmatrix}  $$ =
$$
\text{Det} \left( \begin{pmatrix} 6 & 9 \\ 2 & 3 \end{pmatrix} \right) = (6)(3) - (9)(2) = 18 - 18 = 0
$$
$$
\boxed{0}
$$

### d)
### d)

$$
D = \begin{bmatrix}
0 & 5 \\
-5 & 0 \\
\end{bmatrix}
$$

$$
\text{Det} \left( \begin{pmatrix} 0 & -5 \\ 5 & 0 \end{pmatrix} \right) = (0)(0) - (-5)(5) = 0 + 25 = 25
$$

---

# Ejercicio 2: Cofactores y metodo Sarrus

## Objetivo del ejercicio:

El objetivo es comprender y dominar el cálculo de cofactores y el método de Sarrus para matrices 3x3, con el fin de aplicar estos conceptos en la resolución de determinantes y sistemas de ecuaciones lineales, y así poder manipular y analizar matrices de manera más efectiva en diversos contextos matemáticos.

Dadas las matrices utiliza el metodo sarrus:
### A) Primera matriz
$$
A = \begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 4 \\
5 & 6 & 0
\end{pmatrix}
$$

### Paso 1: Repetir las dos primeras columnas a la derecha

Según la regla de Sarrus, debemos repetir las dos primeras columnas a la derecha de la matriz, como sigue:

$$
\begin{pmatrix}
1 & 2 & 3 & | & 1 & 2 \\
0 & 1 & 4 & | & 0 & 1 \\
5 & 6 & 0 & | & 5 & 6
\end{pmatrix}
$$

### Paso 2: Sumar los productos de las diagonales principales

Ahora calculamos la suma de los productos de las diagonales principales, que van de izquierda a derecha:

- Primera diagonal: ( (1)(1)(0) = 0 )
- Segunda diagonal: ( (2)(4)(5) = 40 )
- Tercera diagonal: ( (3)(0)(6) = 0 )

Sumamos estos productos:

$$
0 + 40 + 0 = 40
$$

### Paso 3: Restar los productos de las diagonales secundarias

Luego, calculamos los productos de las diagonales secundarias, que van de derecha a izquierda:

- Primera diagonal secundaria: ( (3)(1)(5) = 15 )
- Segunda diagonal secundaria: ( (6)(4)(1) = 24 )
- Tercera diagonal secundaria: ( (0)(0)(2) = 0 )

Sumamos estos productos:

$$
15 + 24 + 0 = 39
$$

### Paso 4: Determinante

El determinante es la diferencia entre la suma de las diagonales principales y las secundarias:

$$
\text{Det}(A) = 40 -39 = 1
$$

### Resultado final:

El determinante de la matriz \( A \) es:

$$
\boxed{1}
$$

### B) Segunda matriz 3x3:

$$
B = \begin{pmatrix}
2 & -1 & 3 \\
1 & 4 & 0 \\
3 & 2 & -2
\end{pmatrix}
$$

### Paso 1: Repetir las dos primeras columnas a la derecha

Según la regla de Sarrus, debemos repetir las dos primeras columnas a la derecha de la matriz, como sigue:

$$
\begin{pmatrix}
2 & -1 & 3 & | & 2 & -1 \\
1 & 4 & 0 & | & 1 & 4 \\
3 & 2 & -2 & | & 3 & 2
\end{pmatrix}
$$

### Paso 2: Sumar los productos de las diagonales principales

Ahora calculamos la suma de los productos de las diagonales principales, que van de izquierda a derecha:

- Primera diagonal: ( (2)(4)(-2) = -16 )
- Segunda diagonal: ( (-1)(0)(3) = 0 )
- Tercera diagonal: ( (3)(1)(2) = 6 )

Sumamos estos productos:

$$
-16 + 0 + 6 = -10
$$

### Paso 3: Restar los productos de las diagonales secundarias

Luego, calculamos los productos de las diagonales secundarias, que van de derecha a izquierda:

- Primera diagonal secundaria: ( (3)(4)(3) = 36 )
- Segunda diagonal secundaria: ( (-2)(0)(2) = 0 )
- Tercera diagonal secundaria: ( (-2)(1)(-1) = 2 )

Sumamos estos productos:

$$
36 + 0 + (2) = 38
$$

### Paso 4: Determinante

El determinante es la diferencia entre la suma de las diagonales principales y las secundarias:

$$
\text{Det}(A) = -10 - 38 = -48
$$

### Resultado final:

$$
\boxed{-48}
$$

----
### Ejercicio de Cofactor
$$
C = \begin{pmatrix}
1 & 0 & 2 \\
-1 & 3 & 1 \\
2 & 0 & 1
\end{pmatrix}
$$
### Paso 1: Expansión de cofactores

El determinante de una matriz 3x3 se puede calcular usando la expansión de cofactores a lo largo de la primera fila (o cualquier fila o columna). 
La fórmula general es:

$$
\text{Det}(A) = a_{11} \cdot \text{Cofactor} + a_{12} \cdot \text{Cofactor} + a_{13} \cdot \text{Cofactor}
$$

Donde \(a_{ij}\) son los elementos de la matriz, y los cofactores correspondientes se calculan como:

$$
\text{Cofactor} = (-1)^{i+j} \cdot \text{Det}(\text{Matriz menor})
$$

Donde la "matriz menor" es la matriz resultante al eliminar la fila \(i\) y la columna \(j\).

### Paso 2: Calcular los cofactores

#### Cofactor 1:

El cofactor correspondiente al elemento \( a_11 = 1 \) se obtiene al eliminar la primera fila y la primera columna de la matriz, obteniendo la siguiente matriz menor:

$$
\begin{pmatrix}
3 & 1 \\
0 & 1
\end{pmatrix}
$$

El determinante de esta matriz menor es:

$$
\text{Det} = (3)(1) - (1)(0) = 3
$$

Por lo tanto, el cofactor 1 es:

$$
\text{Cofactor} = (-1)^{1+1} \cdot 3 = 3
$$

#### Cofactor 2:

El cofactor correspondiente al elemento \( a_12= 0 \) se obtiene al eliminar la primera fila y la segunda columna de la matriz, obteniendo la siguiente matriz menor:

$$
\begin{pmatrix}
-1 & 1 \\
2 & 1
\end{pmatrix}
$$

El determinante de esta matriz menor es:

$$
\text{Det} = (-1)(1) - (1)(2) = -1 - 2 = -3
$$

Por lo tanto, el cofactor 2 es:

$$
\text{Cofactor} = (-1)^{1+2} \cdot (-3) = 3
$$

#### Cofactor 3:

El cofactor correspondiente al elemento \( a_13 = 2 \) se obtiene al eliminar la primera fila y la tercera columna de la matriz, obteniendo la siguiente matriz menor:

$$
\begin{pmatrix}
-1 & 3 \\
2 & 0
\end{pmatrix}
$$

El determinante de esta matriz menor es:

$$
\text{Det} = (-1)(0) - (3)(2) = 0 - 6 = -6
$$

Por lo tanto, el cofactor 3 es:

$$
\text{Cofactor} = (-1)^{1+3} \cdot (-6) = -6
$$

### Paso 3: Determinante de la matriz

Ahora, sumamos los productos de los elementos de la primera fila con los cofactores correspondientes:

$$
\text{Det}(A) = (1)(3) + (0)(3) + (2)(-6) = 3 + 0 - 12 = -9
$$

### Resultado final:

El determinante de la matriz \( A \) es:

$$
\boxed{-9}
$$



---

# Ejercicio 3:  Aplicacion a vectores y propidades

## Objetivo del ejercicio:
El objetivo es calcular el **determinante de la matriz 2x2** formada por dos **vectores** dados. Esto permite entender cómo los vectores pueden ser representados como matrices y cómo su determinante refleja propiedades geométricas, como el área del paralelogramo formado por los vectores. Este cálculo es una forma directa de aplicar álgebra lineal a problemas geométricos sencillos.

---
### Verificacion de propiedades
Dadas las matrices:

$$
A = \begin{pmatrix} 
2 & 1 \\
1 & 3 
\end{pmatrix}, \quad 
B = \begin{pmatrix} 
1 & 2 \\
3 & 1 
\end{pmatrix}
$$

### Propiedad 1: ∆(AB) = ∆(A)*∆(B)

#### Paso 1: Calcular ∆(A)

$$
\text{det}(A) = (2)(3) - (1)(1) = 6 - 1 = 5
$$

#### Paso 2: Calcular ∆(B)
$$
\text{det}(B) = (1)(1) - (2)(3) = 1 - 6 = -5
$$

#### Paso 3: Calcular ∆\( AB \)

Multiplicamos \( A \) y \( B \):

$$
AB = \begin{pmatrix} 
2 & 1 \\
1 & 3 
\end{pmatrix}
\begin{pmatrix} 
1 & 2 \\
3 & 1 
\end{pmatrix}
= \begin{pmatrix} 
5 & 5 \\
10 & 5 
\end{pmatrix}
$$

#### Paso 4: Calcular ∆(AB)

$$
\text{det}(AB) = (5)(5) - (5)(10) = 25 - 50 = -25
$$

#### Paso 5: Comparar ambos ∆

$$
\text{det}(A) \cdot \text{det}(B) = 5 \cdot (-5) = -25
$$

Por lo tanto, se cumple:

$$
\text{det}(AB) = \text{det}(A) \cdot \text{det}(B)
$$

### Propiedad 2: ∆(A^T) = ∆(A)
#### Paso 1: Calcular ∆\( A^T \)

La matriz transpuesta de \( A \) es:

$$
A^T = \begin{pmatrix} 
2 & 1 \\
1 & 3 
\end{pmatrix}
$$

#### Paso 2: Calcular A^T

Dado que \( A^T = A \), tenemos que:

$$
\text{det}(A^T) = \text{det}(A) = 5
$$

Por lo tanto, se cumple:

$$
\text{det}(A^T) = \text{det}(A)
$$

---

### Determinante de una matriz 2x2 formada por vectores

Se tienen los vectores:

$$
\mathbf{u} = (3, 2), \quad \mathbf{v} = (1, 4)
$$

### Paso 1: Formar la matriz 2x2
Colocamos los vectores como **columnas** de una matriz 2x2:

$$
A = \begin{pmatrix}
3 & 2 \\
1 & 4
\end{pmatrix}
$$

  ### Paso 2: Calcular el determinante

El determinante de una matriz 2x2 se calcula con la fórmula:

$$
\text{Det}(A) = (3)(4) - (1)(2)
$$

### Paso 3: Resolución

Realizamos la operación:

$$
\text{Det}(A) = 12 - 2 = 10
$$

### Resultado final

El determinante de la matriz \( A \) es:

$$
\boxed{10}
$$

### A) **Calcular el área del paralelogramo que forman los vectores**

El área del paralelogramo formado por dos vectores u e v en el plano es igual al valor absoluto del determinante de la matriz que tiene como columnas esos vectores. En este caso, el determinante de la matriz es 10, por lo tanto:

$$
\text{Área} = |\text{Det}(A)| = |10| = 10
$$

Por lo tanto, el área del paralelogramo formado por los vectores es:

$$
\boxed{10}
$$

---

### B) **Cambiar el área si intercambias los vectores**

Si intercambiamos los vectores, cambiamos la matriz de la siguiente manera:

$$
A' = \begin{pmatrix}
1 & 3 \\
4 & 2
\end{pmatrix}
$$

Ahora calculamos el determinante de la nueva matriz:

$$
\text{Det}(A') = (1)(2) - (3)(4) = 2 - 12 = -10
$$

El **área** sigue siendo el valor absoluto del determinante:

$$
\text{Área} = |\text{Det}(A')| = |-10| = 10
$$

Por lo tanto, aunque el determinante cambie de signo, el **área** del paralelogramo sigue siendo la misma:

$$
\boxed{10}
$$

---

### C) **¿Qué representa el signo del determinante?**

El signo del determinante de la matriz formada por los vectores tiene una interpretación geométrica relacionada con la **orientación** de los vectores. Lo unico que estaria cambiando es su orientacion en el espacio, si esta mirando hacia arriba o hacia abajo.

- Si el **determinante es positivo**, los vectores forman un paralelogramo con una **orientación positiva** (en sentido antihorario).
- Si el **determinante es negativo**, los vectores forman un paralelogramo con una **orientación negativa** (en sentido horario).
---

**Conclusión:** Para esta actividad se me complicaba tener un orden de mis resultados, ya que al realizar varias multiplicaciones, sumas y restas se me olvidaba que seguí, pero con la práctica sé que podré resolverlos más rápido. así mismo se me ha complicado un poco acomodar en este código la manera en como acomodar los aejercicios y diagonales.
