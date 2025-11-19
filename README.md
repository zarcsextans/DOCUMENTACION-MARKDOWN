# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Scarlet Angelina Ruelas Cardeña
## Actividad \#18 - Matrices doc
## Fecha: 18/Octubre/2025
## Descripción: En esta actividad se modificará el código utilizando formato Markdown de manera que al ejecutarlo se muestre los cambios del documento con los datos personales y de la materia a la vez que resolvemos los ejercicios de la clase anterior.
# Determinantes de Matrices 2×2  
Este documento explica paso a paso cómo se calculan los determinantes de varias matrices 2×2.

La fórmula general para una matriz:

\[
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
\]

es:

\[
\text{det} = a \cdot d - b \cdot c
\]

---

##  Matriz A
\[
A =
\begin{pmatrix}
5 & 2 \\
3 & 1
\end{pmatrix}
\]

### Sustitución en la fórmula:
- \(a = 5\)
- \(b = 2\)
- \(c = 3\)
- \(d = 1\)

### Cálculo:
- \(a \cdot d = 5 \cdot 1 = 5\)
- \(b \cdot c = 2 \cdot 3 = 6\)

\[
\text{det}(A) = 5 - 6 = -1
\]

---

##  Matriz B
\[
B =
\begin{pmatrix}
-1 & 4 \\
2 & -8
\end{pmatrix}
\]

### Sustitución:
- \(a = -1\)
- \(b = 4\)
- \(c = 2\)
- \(d = -8\)

### Cálculo:
- \(a \cdot d = -1 \cdot -8 = 8\)
- \(b \cdot c = 4 \cdot 2 = 8\)

\[
\text{det}(B) = 8 - 8 = 0
\]

---

##  Matriz C
\[
C =
\begin{pmatrix}
6 & 9 \\
2 & 3
\end{pmatrix}
\]

### Sustitución:
- \(a = 6\)
- \(b = 9\)
- \(c = 2\)
- \(d = 3\)

### Cálculo:
- \(a \cdot d = 6 \cdot 3 = 18\)
- \(b \cdot c = 9 \cdot 2 = 18\)

\[
\text{det}(C) = 18 - 18 = 0
\]

---

##  Matriz D
\[
D =
\begin{pmatrix}
0 & 5 \\
-5 & 0
\end{pmatrix}
\]

### Sustitución:
- \(a = 0\)
- \(b = 5\)
- \(c = -5\)
- \(d = 0\)

### Cálculo:
- \(a \cdot d = 0 \cdot 0 = 0\)
- \(b \cdot c = 5 \cdot -5 = -25\)

\[
\text{det}(D) = 0 - (-25) = 25
\]

---
===========================================
EJERCICIO 2: Cálculo de determinantes 3×3
Regla de Sarrus
===========================================

===========================================
MATRIZ E
===========================================

| 1   2   3 |
| 0   1   4 |
| 5   6   0 |

### Paso 1: Repetimos las dos primeras columnas
| 1   2   3 | 1   2 |
| 0   1   4 | 0   1 |
| 5   6   0 | 5   6 |

### Paso 2: Diagonales principales 
1) 1 * 1 * 0 = 0
2) 2 * 4 * 5 = 40
3) 3 * 0 * 6 = 0

Suma de diagonales principales:
Dp = 40

### Paso 3: Diagonales secundarias 
1) 3 * 1 * 5 = 15
2) 2 * 0 * 0 = 0
3) 1 * 4 * 6 = 24

Suma de diagonales secundarias:
Ds = 39

### Paso 4: Determinante final
Det(E) = Dp - Ds = 40 - 39 = 1


===========================================
MATRIZ F
===========================================

| 2  -1   3 |
| 1   4   0 |
| 3   2  -2 |

### Paso 1: Repetimos las dos primeras columnas
| 2  -1   3 | 2  -1 |
| 1   4   0 | 1   4 |
| 3   2  -2 | 3   2 |

### Paso 2: Diagonales principales 
1) 2 * 4 * (-2) = -16
2) -1 * 0 * 3   = 0
3) 3 * 1 * 2    = 6

Suma de diagonales principales:
Dp = -10

### Paso 3: Diagonales secundarias 
1) 3 * 4 * 3 = 36
2) -1 * 1 * (-2) = 2
3) 2 * 0 * 2 = 0

Suma de diagonales secundarias:
Ds = 38

### Paso 4: Determinante final
Det(F) = Dp - Ds = -10 - 38 = -48

