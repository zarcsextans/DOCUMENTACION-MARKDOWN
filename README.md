# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Scarlet Angelina Ruelas Cardeña
## Actividad \#16 - Matrices doc
## Fecha: 11/Noviembre/2025
## Descripción: En esta actividad se modificará el código utilizando formato Markdown de manera que al ejecutarlo se muestre los cambios del documento con los datos personales y de la materia a la vez que resolvemos los ejercicios.
---
### Ejercicio 1: Clasificar matrices  

Identifica el tipo de cada matriz:

```math
A = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix},\quad
B = \begin{pmatrix} 3 & 0 & 0 \\ 0 & -2 & 0 \\ 0 & 0 & 5 \end{pmatrix},\quad
C = \begin{pmatrix} 2 & 1 & 4 \\ 1 & 3 & 5 \\ 4 & 5 & 6 \end{pmatrix},\quad
D = \begin{pmatrix} 1 & 2 & 3 \\ 0 & 4 & 5 \\ 0 & 0 & 6 \end{pmatrix}
```

---

#### Matriz A  
Matriz **identidad** $I_2$, también es **diagonal**, **escalar** ($\lambda = 1$), **simétrica** y **triangular superior e inferior**.  
Propiedad: $A = A^T$.

---

#### Matriz B  
Matriz **diagonal** de orden $3 \times 3$.  
También es **triangular superior e inferior**, y **simétrica**.  
No es escalar porque sus elementos diagonales son diferentes $(3, -2, 5)$.

---

#### Matriz C  
Matriz **simétrica** de orden $3 \times 3$.  
Se cumple que $C_{ij} = C_{ji}$ (por ejemplo: $C_{12}=1=C_{21}$, $C_{13}=4=C_{31}$, $C_{23}=5=C_{32}$).  
No es diagonal ni triangular.

---

#### Matriz D  
Matriz **triangular superior** de orden $3 \times 3$.  
No es simétrica ni diagonal.  
Su determinante es:

```math
\det(D) = 1 \cdot 4 \cdot 6 = 24 \neq 0
```

Por lo tanto, es **invertible**.

---

### Conclusión del Ejercicio 1  

En este ejercicio se identificaron los distintos tipos de matrices según sus elementos y posición de los ceros.  
Se reconocieron las propiedades que distinguen a las matrices identidad, diagonal, simétrica y triangular, fundamentales para la manipulación algebraica de matrices.

---

### Ejercicio 2: Operaciones básicas  

Dadas las matrices:

```math
A = \begin{pmatrix} 2 & -1 \\ 3 & 4 \end{pmatrix},\quad
B = \begin{pmatrix} 5 & 2 \\ -1 & 3 \end{pmatrix}
```

Calcula:  
a) $A + B$  
b) $2A - B$  
c) $AB$  
d) $BA$  
e) $A^T$

---

#### a) Suma de matrices $A + B$

```math
A + B
= \begin{pmatrix} 2+5 & -1+2 \\ 3+(-1) & 4+3 \end{pmatrix}
= \begin{pmatrix} 7 & 1 \\ 2 & 7 \end{pmatrix}
```

---

#### b) Operación $2A - B$

```math
2A - B
= 2\begin{pmatrix} 2 & -1 \\ 3 & 4 \end{pmatrix}
  - \begin{pmatrix} 5 & 2 \\ -1 & 3 \end{pmatrix}
= \begin{pmatrix} 4 & -2 \\ 6 & 8 \end{pmatrix}
  - \begin{pmatrix} 5 & 2 \\ -1 & 3 \end{pmatrix}
= \begin{pmatrix} -1 & -4 \\ 7 & 5 \end{pmatrix}
```

---

#### c) Producto $AB$

```math
AB
= \begin{pmatrix} 2 & -1 \\ 3 & 4 \end{pmatrix}
  \begin{pmatrix} 5 & 2 \\ -1 & 3 \end{pmatrix}
= \begin{pmatrix}
  (2)(5)+(-1)(-1) & (2)(2)+(-1)(3) \\
  (3)(5)+(4)(-1)  & (3)(2)+(4)(3)
  \end{pmatrix}
= \begin{pmatrix} 11 & 1 \\ 11 & 18 \end{pmatrix}
```

---

#### d) Producto $BA$

```math
BA
= \begin{pmatrix} 5 & 2 \\ -1 & 3 \end{pmatrix}
  \begin{pmatrix} 2 & -1 \\ 3 & 4 \end{pmatrix}
= \begin{pmatrix}
  (5)(2)+(2)(3) & (5)(-1)+(2)(4) \\
  (-1)(2)+(3)(3) & (-1)(-1)+(3)(4)
  \end{pmatrix}
= \begin{pmatrix} 16 & 3 \\ 7 & 13 \end{pmatrix}
```

---

#### e) Transpuesta de $A$

```math
A^T
= \begin{pmatrix} 2 & -1 \\ 3 & 4 \end{pmatrix}^T
= \begin{pmatrix} 2 & 3 \\ -1 & 4 \end{pmatrix}
```

---

### Conclusión del Ejercicio 2  

Se aplicaron operaciones básicas entre matrices: suma, resta, multiplicación y transposición.  
Se comprobó que el producto de matrices **no es conmutativo** ($AB \neq BA$) y que la transpuesta convierte filas en columnas.

---

### Ejercicio 3: Multiplicación en cadena  

Dadas las matrices:

```math
A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix},\quad
B = \begin{pmatrix} 2 & 0 \\ 1 & 3 \end{pmatrix},\quad
C = \begin{pmatrix} 1 & 1 \\ 0 & 2 \end{pmatrix}
```

Verifica que $(AB)C = A(BC)$

---

#### Paso 1: Calcular \(AB\)

```math
AB
= \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}
  \begin{pmatrix} 2 & 0 \\ 1 & 3 \end{pmatrix}
= \begin{pmatrix}
  (1)(2)+(2)(1) & (1)(0)+(2)(3) \\
  (3)(2)+(4)(1) & (3)(0)+(4)(3)
  \end{pmatrix}
= \begin{pmatrix} 4 & 6 \\ 10 & 12 \end{pmatrix}
```

---

#### Paso 2: Calcular \((AB)C\)

```math
(AB)C
= \begin{pmatrix} 4 & 6 \\ 10 & 12 \end{pmatrix}
  \begin{pmatrix} 1 & 1 \\ 0 & 2 \end{pmatrix}
= \begin{pmatrix}
  (4)(1)+(6)(0) & (4)(1)+(6)(2) \\
  (10)(1)+(12)(0) & (10)(1)+(12)(2)
  \end{pmatrix}
= \begin{pmatrix} 4 & 16 \\ 10 & 34 \end{pmatrix}
```

---

#### Paso 3: Calcular \(BC\)

```math
BC
= \begin{pmatrix} 2 & 0 \\ 1 & 3 \end{pmatrix}
  \begin{pmatrix} 1 & 1 \\ 0 & 2 \end{pmatrix}
= \begin{pmatrix}
  (2)(1)+(0)(0) & (2)(1)+(0)(2) \\
  (1)(1)+(3)(0) & (1)(1)+(3)(2)
  \end{pmatrix}
= \begin{pmatrix} 2 & 2 \\ 1 & 7 \end{pmatrix}
```

---

#### Paso 4: Calcular \(A(BC)\)

```math
A(BC)
= \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}
  \begin{pmatrix} 2 & 2 \\ 1 & 7 \end{pmatrix}
= \begin{pmatrix}
  (1)(2)+(2)(1) & (1)(2)+(2)(7) \\
  (3)(2)+(4)(1) & (3)(2)+(4)(7)
  \end{pmatrix}
= \begin{pmatrix} 4 & 16 \\ 10 & 34 \end{pmatrix}
```

---

#### Verificación  

```math
(AB)C = \begin{pmatrix} 4 & 16 \\ 10 & 34 \end{pmatrix},\quad
A(BC) = \begin{pmatrix} 4 & 16 \\ 10 & 34 \end{pmatrix}
```

Por lo tanto:

```math
(AB)C = A(BC)
```

---

### Conclusión del Ejercicio 3  

Se verificó la **propiedad asociativa** de la multiplicación de matrices: $(AB)C = A(BC)$.  
Esta propiedad permite reorganizar multiplicaciones en cadena sin alterar el resultado.

---
