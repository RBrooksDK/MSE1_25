---
tags:
    - Linear algebra
    - Systems of linear equations
    - Row reduction
    - Echelon form
    - Reduced row echelon form
    - Matrix operations
    - Matrices
---

<h1 align="center">Introduction to Linear Algebra</h1>

### Session Preparation:

Brooks: [Chapter 7](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/RBrooksDK/MSE_book_v2/master/main.pdf)

Some of the exercises may require you to use Python. You may also need to install the `numpy` and `sympy` libraries if you haven't already.

### Resources Danish Class:

[Session notes](https://drive.google.com/file/d/1pfrbRf2fb2jAqhIg1xhlJw0KHmDjXqds/view?usp=sharing)

[Session Resources](https://viaucdk-my.sharepoint.com/:f:/g/personal/rib_viauc_dk/EkjUOJhNa7lFscFUs9rWtwsB_2p-THcKaRcRj3M3LYR99g?e=LzRrSp)

### Exercises

#### Exercise 1: Echelon and Reduced Echelon Form
Determine whether the following matrices are in reduced echelon form, echelon form, or neither.

a. $\begin{bmatrix} 1 & 0 & 2 & 1\\ 
                0 & 1 & -3 & 0\end{bmatrix}$

b.
$\begin{bmatrix} 1 & 2 & -2 & 5\\
                0 & 1 &  0 & -1\\
                0 & 0 &  1 & 3 \\ 
                0 & 0 &  0 & 1\end{bmatrix}$

c.
$\begin{bmatrix} -1 & 0\\
                0 & 4\\
                0 & 0 \end{bmatrix}$

d.
$\begin{bmatrix} 1 & 0 & 1 & 0 & -1\\
                0 & 1 & 1 & 0 & 0\\
                0 & 0 & 0 & 0 & 0\\
                0 & 0 & 0 & 1 & -1\end{bmatrix}$

e.
$\begin{bmatrix} 0 & 3 & 0 & 4\\
                0 & 0 & -2 & -2\\
                0 & 0 & 0 & 7\end{bmatrix}$

f.
$\begin{bmatrix} 1 & 0 & 0 & 1\\
                0 & 0 & 1 & -2\\
                0 & 0 & 0 & 1\end{bmatrix}$

??? answer "&nbsp;"
    a. reduced echelon form 

    b. echelon form

    c. echelon form

    d. neither

    e. echelon form

    f. echelon form



#### Exercise 2: Row operations
Explain which row operations are used in the calculations below.

a.
$\begin{bmatrix}
    4 & -3 & 1 & 2 \\
    3 & 1 & -5 & 6 \\
    1 & 1 & 2 & 4 \\
    \end{bmatrix}
    \sim
\begin{bmatrix}
    1 & 1 & 2 & 4 \\
    3 & 1 & -5 & 6 \\
    4 & -3 & 1 & 2 \\
    \end{bmatrix}$

??? answer "&nbsp;"
    Swap: $r_1 \leftrightarrow r_3$

b. $\begin{bmatrix}
    1 & 1 & 2 & 4 \\
    3 & 1 & -5 & 6 \\
    4 & -3 & 1 & 2 \\
    \end{bmatrix}
    \sim
    \begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & -2 & -11 & -6 \\
    4 & -3 & 1 & 2 \\
    \end{bmatrix}$

??? answer "&nbsp;"
    Replacement: $r_2 \rightarrow r_2 - 3r_1$
c. $\begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & -2 & -11 & -6 \\
    4 & -3 & 1 & 2 \\
    \end{bmatrix}
    \sim
    \begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & -2 & -11 & -6 \\
    0 & -7 & -7 & -14 \\
    \end{bmatrix}$

??? answer "&nbsp;"
    Replacement: $r_3 \rightarrow r_3 - 4r_1$

d. $\begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & -2 & -11 & -6 \\
    0 & -7 & -7 & -14 \\
    \end{bmatrix}
    \sim
    \begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & -2 & -11 & -6 \\
    0 & 1 & 1 & 2 \\
    \end{bmatrix}$

??? answer "&nbsp;"

    Scaling: $r_3 \rightarrow -\frac{1}{7}r_3$

e. $\begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & -2 & -11 & -6 \\
    0 & 1 & 1 & 2 \\
    \end{bmatrix}
    \sim
    \begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & 1 & 1 & 2 \\
    0 & -2 & -11 & -6 \\
    \end{bmatrix}$

??? answer "&nbsp;"
    Swap: $r_2 \leftrightarrow r_3$

f. $\begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & 1 & 1 & 2 \\
    0 & -2 & -11 & -6 \\
    \end{bmatrix}
    \sim
    \begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & 1 & 1 & 2 \\
    0 & 0 & -9 & -2 \\
    \end{bmatrix}$

??? answer "&nbsp;"
    Replacement: $r_3 \rightarrow r_3 + 2r_2$

g. The reduced matrix from (f)  is the augmented matrix for a system of linear equations. Does this system have no solution, a unique solution, or infinitely many solutions?

??? answer "&nbsp;"
    The system has a unique solution, since there is a pivot in each column of the coefficient part of the reduced matrix.

#### Exercise 3: System of linear equations
Given the following system of linear equations:

$$
\begin{aligned}
2x_1 - 4x_2 + 6x_3 &= 2 \\
x_1 + x_3 &= 3 \\
-4x_1 + 2x_2 &= 2
\end{aligned}
$$

a. Write down the augmented matrix for the system.

??? answer "&nbsp;"
    $\begin{bmatrix}
    2 & -4 & 6 & 2\\
    1 & 0  & 1 & 3\\
    -4& 2  & 0 & 2
    \end{bmatrix}$

b. Use row operations to get the reduced row echelon form of the matrix and write down the solution.

??? answer "&nbsp;"
    RREF:
    $\begin{bmatrix}
    1 & 0 & 0 & 1\\
    0 & 1 & 0 & 3\\
    0 & 0 & 1 & 2
    \end{bmatrix}$

    Solution:
    $\begin{cases}
        x_1 = 1\\
        x_2 = 3\\
        x_3 = 2
    \end{cases}$

#### Exercise 4: Row Reduction
Solve the systems whose augmented matrices are given below. Write down the general solution, i.e. write the basic variables in terms of the free variables. 

a. $\begin{bmatrix} 1 & 2 & 3 & 4\\
                    4 & 8 & 9 & 4\end{bmatrix}$

??? answer "&nbsp;"
    $\begin{cases}
        x_1 = -8-2x_2\\
        x_2 \text{ free}\\
        x_3 = 4
    \end{cases}$

b. $\begin{bmatrix} 1 & -1 & -2 & 3\\
                    4 & -2 & -8 & 2\end{bmatrix}$

??? answer "&nbsp;"
    $\begin{cases}
        x_1 = -2+2x_3\\
        x_2 = -5\\
        x_3 \text{ free}
    \end{cases}$

c. $\begin{bmatrix} -2 & 4 & -3 & 0\\
                    4 & -8 & 6& 0\\
                    -6& 12& -9 & 0\end{bmatrix}$

??? answer "&nbsp;"
    $\begin{cases}
        x_1 = 2x_2 - \frac{3}{2}x_3\\
        x_2 \text{ free}\\
        x_3 \text{ free}
    \end{cases}$

#### Exercise 5: Consistency of the system
Which of the augmented matrices below represent an inconsistent system of equations?

a. $\begin{bmatrix}
    0 & 3 & -2 & 1\\
    0 & 0  & -1 & 4\\
    0 & 0  & 0 & 0 \end{bmatrix}$

b. $\begin{bmatrix}
    -1 & 3 & 1 \\
    0 & 5  & 3 \\
    0 & 0  & 6 \end{bmatrix}$

c. $\begin{bmatrix}
    7 & 1 & 1 \\
    0 & 2  & 2 \\
    0 & 0  & 3 \\
    0 & 0  & 0
\end{bmatrix}$

d. $\begin{bmatrix}
    1 & 0 \\
    0 & 1 
\end{bmatrix}$

e. $\begin{bmatrix}
    -3 & 0 & 0 & 9\\
    0 & 1  & 0 & 0\\
    0 & 0  & 4 & 0
\end{bmatrix}$

f. $\begin{bmatrix}
    0 & 0 & 6 & 3
\end{bmatrix}$

??? answer "&nbsp;"
    inconsistent: b, c, d

    consistent: a, e, f


g. For the consistent systems find the general solution.

??? answer "&nbsp;"
    a. $\begin{cases}
        x_1 \text{ free}\\
        x_2 = -\frac{7}{3}\\
        x_3 = -4
    \end{cases}$

    e. $\begin{cases}
        x_1 = - 3\\
        x_2 = 0\\
        x_3 = 0
    \end{cases}$

    f. $\begin{cases}
        x_1 \text{ free}\\
        x_2 \text{ free}\\
        x_3 = \frac{1}{2}
    \end{cases}$


#### Exercise 6: Plan a diet
Use Python to solve this exercise. 

For a week you decide to eat only butter, apples, and oats.

|Nutritional values per 100 g|  Butter  |  Apple  |  Oats  | Rye bread|
|----------------------------|---------:|--------:|-------:|---------:|
|Protein       (g)           |    0.2   |   0.3   | 14.0   |    6.4   |
|Fat           (g)           |   82.5   |   0.2   |  6.9   |    4.7   |
|Carbohydrates (g)           |    0.0   |   12.1  | 57.0   |   32.0   |

a. How much butter, apple, and oats do you need to eat to get 50 g of protein, 70 g of fat, and 260 g of carbohydrates per day?

??? answer "&nbsp;"
    $\begin{cases}  54.7 \text{ g butter}\\
                522.8\text{ g apple}\\
                345.2 \text{ g oats}\end{cases}$


Next week, you decide to replace apples with rye bread.

b. Is it possible to plan a diet of butter, rye bread, and oats to still get 50 g of protein, 70 g of fat and 260 g of carbohydrate per day?

??? answer "&nbsp;"
    No, the system of linear equations has a unique solution. However, the solution contains a negative amount of oats, which does not make sense.