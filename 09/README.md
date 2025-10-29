---
tags:
    - Linear algebra
    - Systems of linear equations
    - Matrix operations
    - Matrices
    - Linear transformations    
    - Determinants
    - Matrix inverses
    - Vector spaces
    - Span
    - Linear independence
    - Invertible matrices
---

<h1 align="center">Matrix Algebra and Determinants</h1>

### Session Preparation

Brooks: [Chapter 9](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/RBrooksDK/MSE_book_v2/master/main.pdf)

Some of the exercises may require you to use Python. You may also need to install the `numpy` and `sympy` libraries if you haven't already.

### Resources Danish Class:

[Session notes](MISSING LINK)

[Session Resources](MISSING LINK)

### Exercises

**[Python]** Means that you are advised to use Python to solve the exercise. You can find the Python solutions [here](https://github.com/RBrooksDK/MSE1_25/blob/main/09/Python_solutions_for_exercises_09.ipynb) or download them [here](Python_solutions_for_exercises_09.ipynb)

#### Exercise 1
1. Determine *by inspection* whether the following sets of vectors are linearly independent or dependent. Justify each answer.
{ .annotate }

    i. $\left[\begin{array}{l}5 \\ 1\end{array}\right],\left[\begin{array}{l}2 \\ 8\end{array}\right],\left[\begin{array}{l}1 \\ 3\end{array}\right],\left[\begin{array}{r}-1 \\ 7\end{array}\right]$ (1)
    { .annotate }

    1. Dependent

    ii. $\left[\begin{array}{r}2 \\ -4 \\ 8\end{array}\right],\left[\begin{array}{r}-3 \\ 6 \\ -12\end{array}\right]$  (1)
    { .annotate }

    1. Dependent

    iii. $\left[\begin{array}{r}5 \\ -3 \\ -1\end{array}\right],\left[\begin{array}{l}0 \\ 0 \\ 0\end{array}\right],\left[\begin{array}{r}-7 \\ 2 \\ 4\end{array}\right]$  (1)
    { .annotate }

    1. Dependent

    iv. $\left[\begin{array}{l}3 \\ 4\end{array}\right],\left[\begin{array}{r}-1 \\ 5\end{array}\right],\left[\begin{array}{l}3 \\ 5\end{array}\right],\left[\begin{array}{l}7 \\ 1\end{array}\right]$  (1)
    { .annotate }

    1. Dependent

    v. $\left[\begin{array}{r}-8 \\ 12 \\ -4\end{array}\right],\left[\begin{array}{r}2 \\ -3 \\ -1\end{array}\right]$  (1)
    { .annotate }

    1. Independent

    vi. $\left[\begin{array}{r}1 \\ 4 \\ -7\end{array}\right],\left[\begin{array}{r}-2 \\ 5 \\ 3\end{array}\right],\left[\begin{array}{l}0 \\ 0 \\ 0\end{array}\right]$  (1)
    { .annotate }

    1. Dependent

2. Let $A = \left[\begin{array}{cccccc}1 & -4 & -2 & 0 & 3 & -5 \\ 0 & 0 & 1 & 0 & 0 & -1 \\ 0 & 0 & 0 & 0 & 1 & -4 \\ 0 & 0 & 0 & 0 & 0 & 0\end{array}\right]$

    Describe all solutions to $A \mathbf{x}=\mathbf{0}$ in parametric form.

    ??? answer "&nbsp;"

        To describe all solutions to $A\mathbf{x}=\mathbf{0}$ in parametric form, we first write the (coefficient) matrix and then reduce it to reduced echelon form:

        $$
        \left[\begin{array}{cccccc}
        1 & -4 & -2 & 0 & 3 & -5  \\
        0 & 0 & 1 & 0 & 0 & -1  \\
        0 & 0 & 0 & 0 & 1 & -4  \\
        0 & 0 & 0 & 0 & 0 & 0 
        \end{array}\right]
        \sim
        \left[\begin{array}{cccccc}
        1 & -4 & 0 & 0 & 0 & 5  \\
        0 & 0 & 1 & 0 & 0 & -1  \\
        0 & 0 & 0 & 0 & 1 & -4  \\
        0 & 0 & 0 & 0 & 0 & 0 
        \end{array}\right]
        $$

        Therefore, the solution in parametric form is:

        $$
        \mathbf{x} = \left[\begin{array}{c}
        x_1 \\
        x_2 \\
        x_3 \\
        x_4 \\
        x_5 \\
        x_6
        \end{array}\right] = x_2 \left[\begin{array}{c}
        4 \\
        1 \\
        0 \\
        0 \\
        0 \\
        0
        \end{array}\right] + x_4 \left[\begin{array}{c}
        0 \\
        0 \\
        0 \\
        1 \\
        0 \\
        0
        \end{array}\right] + x_6 \left[\begin{array}{c}
        -5 \\
        0 \\
        1 \\
        0 \\
        4 \\
        1
        \end{array}\right]
        $$

        where $x_2$, $x_4$, and $x_6$ are free variables.

3. **[Python]** Use as many columns of $A$ as possible to construct a matrix $B$ with the property that the equation $B \mathbf{x}=\mathbf{0}$ has only the trivial solution. Solve $B \mathbf{x}=\mathbf{0}$ to verify your work.

$A=\left[\begin{array}{rrrrr}3 & -4 & 10 & 7 & -4 \\ -5 & -3 & -7 & -11 & 15 \\ 4 & 3 & 5 & 2 & 1 \\ 8 & -7 & 23 & 4 & 15\end{array}\right]$

??? answer "&nbsp;"

    When reduced to echelon form, you will have pivots in columns, 1, 2, and 4. Therefore, you can use columns 1, 2, and 4 to construct matrix B.

    You can verify your work by solving the equation $B \mathbf{x}=\mathbf{0}$ which is done by finding reduced echelon form of $B$. This will give you the trivial solution.

#### Exercise 2

In (a) and (b) compute each matrix sum or product if it is defined. If an expression is undefined, explain why. Let

$$
\begin{aligned}
& A=\left[\begin{array}{rrr}
2 & 0 & -1 \\
4 & -5 & 2
\end{array}\right], \quad B=\left[\begin{array}{rrr}
7 & -5 & 1 \\
1 & -4 & -3
\end{array}\right], \\
& C=\left[\begin{array}{rr}
1 & 2 \\
-2 & 1
\end{array}\right], \quad D=\left[\begin{array}{rr}
3 & 5 \\
-1 & 4
\end{array}\right], \quad E=\left[\begin{array}{r}
-5 \\
3
\end{array}\right]
\end{aligned}
$$

1. $-2 A, \; B-2 A, \; A C, \; C D$

    ??? answer "&nbsp;"

        $-2 A=(-2)\left[\begin{array}{rrr}2 & 0 & -1 \\ 4 & -5 & 2\end{array}\right]=\left[\begin{array}{rrr}-4 & 0 & 2 \\ -8 & 10 & -4\end{array}\right]$. Next, use $B-2 A=B+(-2 A)$ :

        $$
            B-2 A=\left[\begin{array}{rrr}
        7 & -5 & 1 \\
        1 & -4 & -3
        \end{array}\right]+\left[\begin{array}{rrr}
        - 4 & 0 & 2 \\
        -8 & 10 & -4
        \end{array}\right]=\left[\begin{array}{rrr}
        3 & -5 & 3 \\
        -7 & 6 & -7
        \end{array}\right]
        $$


        The product $A C$ is not defined because the number of columns of $A$ does not match the number of rows of $C . C D=\left[\begin{array}{rr}1 & 2 \\ -2 & 1\end{array}\right]\left[\begin{array}{rr}3 & 5 \\ -1 & 4\end{array}\right]=\left[\begin{array}{rr}1 \cdot 3+2(-1) & 1 \cdot 5+2 \cdot 4 \\ -2 \cdot 3+1(-1) & -2 \cdot 5+1 \cdot 4\end{array}\right]=\left[\begin{array}{rr}1 & 13 \\ -7 & -6\end{array}\right]$. For mental computation, the row-column rule is probably easier to use than the definition.


2. **[Python]** $A+3 B, \; 2 C-3 E, \; D B, \; E C$

    ??? answer "&nbsp;"

        $$
        A+3 B=\left[\begin{array}{rrr}
        2 & 0 & -1 \\
        4 & -5 & 2
        \end{array}\right]+3\left[\begin{array}{rrr}
        7 & -5 & 1 \\
        1 & -4 & -3
        \end{array}\right]=\left[\begin{array}{rrr}
        2+21 & 0-15 & -1+3 \\
        4+3 & -5-12 & 2-9
        \end{array}\right]=\left[\begin{array}{rrr}
        23 & -15 & 2 \\
        7 & -17 & -7
        \end{array}\right]
        $$

        The expression $2 C-3 E$ is not defined because $2 C$ has 2 columns and $-3 E$ has only 1 column.

        $$
        D B=\left[\begin{array}{rr}
        3 & 5 \\
        -1 & 4
        \end{array}\right]\left[\begin{array}{rrr}
        7 & -5 & 1 \\
        1 & -4 & -3
        \end{array}\right]=\left[\begin{array}{rrr}
        3 \cdot 7+5 \cdot 1 & 3(-5)+5(-4) & 3 \cdot 1+5(-3) \\
        -1 \cdot 7+4 \cdot 1 & -1(-5)+4(-4) & -1 \cdot 1+4(-3)
        \end{array}\right]=\left[\begin{array}{rrr}
        26 & -35 & -12 \\
        -3 & -11 & -13
        \end{array}\right]
        $$

        The product $E C$ is not defined because the number of columns of $E$ does not match the number of rows of $C$.

3. **[Python]** Let $A=\left[\begin{array}{rr}3 & -6 \\ -1 & 2\end{array}\right], B=\left[\begin{array}{rr}-1 & 1 \\ 3 & 4\end{array}\right]$, and $C= \left[\begin{array}{rr}-3 & -5 \\ 2 & 1\end{array}\right]$. Verify that $A B=A C$ and yet $B \neq C$.

    ??? answer "&nbsp;"

        To verify that \( AB = AC \) but \( B \neq C \), we compute \( AB \) and \( AC \) and compare them.

        Given:

        $$
        A = \left[\begin{array}{rr} 3 & -6 \\ -1 & 2 \end{array}\right], \quad B = \left[\begin{array}{rr} -1 & 1 \\ 3 & 4 \end{array}\right], \quad C = \left[\begin{array}{rr} -3 & -5 \\ 2 & 1 \end{array}\right]
        $$

        **Compute \( AB \):**
    
        $$
        AB = \left[\begin{array}{rr} 3 & -6 \\ -1 & 2 \end{array}\right] \left[\begin{array}{rr} -1 & 1 \\ 3 & 4 \end{array}\right] = \left[\begin{array}{rr} -21 & -21 \\ 7 & 7 \end{array}\right]
        $$

        **Compute \( AC \):**

        \[
        AC = \left[\begin{array}{rr} 3 & -6 \\ -1 & 2 \end{array}\right] \left[\begin{array}{rr} -3 & -5 \\ 2 & 1 \end{array}\right] = \left[\begin{array}{rr} -21 & -21 \\ 7 & 7 \end{array}\right]
        \]

        Since \( AB = \left[\begin{array}{rr} -21 & -21 \\ 7 & 7 \end{array}\right] = AC \), we conclude \( AB = AC \).

        Thus, \( AB = AC \) but \( B \neq C \).

4. **[Python]** If $A=\left[\begin{array}{rr}1 & -3 \\ -3 & 5\end{array}\right]$ and $A B=\left[\begin{array}{rr}-3 & -11 \\ 1 & 17\end{array}\right]$, determine the matrix $B$.

    ??? answer "&nbsp;"

        Since $\left[\begin{array}{rr}-3 & -11 \\ 1 & 17\end{array}\right]=A B=\left[\begin{array}{ll}A \mathbf{b}_1 & A \mathbf{b}_2\end{array}\right]$, the first column of $B$ satisfies the equation $A \mathbf{x}=\left[\begin{array}{r}-1 \\ 6\end{array}\right]$. Row reduction: $\left[\begin{array}{ll}A & A \mathbf{b}_1\end{array}\right] \sim\left[\begin{array}{rrr}1 & -3 & -3 \\ -3 & 5 & 1\end{array}\right] \sim\left[\begin{array}{lll}1 & 0 & 3 \\ 0 & 1 & 2\end{array}\right]$. So $\mathbf{b}_1=\left[\begin{array}{l}3 \\ 2\end{array}\right]$. Similarly, $\left[\begin{array}{ll}A & A \mathbf{b}_2\end{array}\right] \sim\left[\begin{array}{rrr}1 & -3 & -11 \\ -3 & 5 & 17\end{array}\right] \sim\left[\begin{array}{lll}1 & 0 & 1 \\ 0 & 1 & 4\end{array}\right]$ and $\mathbf{b}_2=\left[\begin{array}{l}1 \\ 4\end{array}\right]$.

        Note: An alternative solution is to row reduce $\left[\begin{array}{lll}A & A \mathbf{b}_1 & A \mathbf{b}_2\end{array}\right]$ with one sequence of row operations. This observation can prepare the way for the inversion algorithm mentioned in the book.

#### Exercise 3

1. Find the inverses of $\begin{array}{cc}{\left[\begin{array}{l}8 \\ 5\end{array}\right.} & \left.\begin{array}{c}6 \\ 4\end{array}\right]\end{array}$ and $\begin{array}{cc}{\left[\begin{array}{l}3 \\ 8\end{array}\right.} & \left.\begin{array}{c}2 \\ 5\end{array}\right]\end{array}$.

    ??? answer "&nbsp;"

        $\left[\begin{array}{ll}8 & 6 \\ 5 & 4\end{array}\right]^{-1}=\frac{1}{32-30}\left[\begin{array}{rr}4 & -6 \\ -5 & 8\end{array}\right]=\left[\begin{array}{cr}2 & -3 \\ -5 / 2 & 4\end{array}\right]$
        
        $\left[\begin{array}{ll}3 & 2 \\ 8 & 5\end{array}\right]^{-1}=\frac{1}{15-16}\left[\begin{array}{rr}5 & -2 \\ -8 & 3\end{array}\right]=\left[\begin{array}{cc}-5 & 2 \\ 8 & -3\end{array}\right]$

2. **[Python]** Use the inverse found in Exercise 3.a to solve the system

    $\begin{aligned}
    & 8 x_1+6 x_2=2 \\
    & 5 x_1+4 x_2=-1
    \end{aligned}$

    ??? answer "&nbsp;"
        The system is equivalent to $A \mathbf{x}=\mathbf{b}$, where $A=\left[\begin{array}{ll}8 & 6 \\ 5 & 4\end{array}\right]$ and $\mathbf{b}=\left[\begin{array}{r}2 \\ -1\end{array}\right]$, and the solution is $\mathbf{x}=A^{-1} \mathbf{b}=\left[\begin{array}{cr}2 & -3 \\ -5 / 2 & 4\end{array}\right]\left[\begin{array}{r}2 \\ -1\end{array}\right]=\left[\begin{array}{r}7 \\ -9\end{array}\right]$. Thus $x_1=7$ and $x_2=-9$.

3. **[Python]** Find the inverse of the matrix. Use the algorithm for finding the inverse of a $n \times n$ matrix.

    $\left[\begin{array}{rrr}
    1 & 0 & -2 \\
    -3 & 1 & 4 \\
    2 & -3 & 4
    \end{array}\right]$

    ??? answer "&nbsp;"

        $$
        \begin{aligned}
        & {\left[\begin{array}{ll}
        A & I
        \end{array}\right]=\left[\begin{array}{rrrrrr}
        1 & 0 & -2 & 1 & 0 & 0 \\
        -3 & 1 & 4 & 0 & 1 & 0 \\
        2 & -3 & 4 & 0 & 0 & 1
        \end{array}\right] \sim\left[\begin{array}{rrrrrr}
        1 & 0 & -2 & 1 & 0 & 0 \\
        0 & 1 & -2 & 3 & 1 & 0 \\
        0 & -3 & 8 & -2 & 0 & 1
        \end{array}\right]} \\
        & \sim\left[\begin{array}{rrrrrr}
        1 & 0 & -2 & 1 & 0 & 0 \\
        0 & 1 & -2 & 3 & 1 & 0 \\
        0 & 0 & 2 & 7 & 3 & 1
        \end{array}\right] \sim\left[\begin{array}{rrrrrr}
        1 & 0 & 0 & 8 & 3 & 1 \\
        0 & 1 & 0 & 10 & 4 & 1 \\
        0 & 0 & 2 & 7 & 3 & 1
        \end{array}\right] \\
        & \sim\left[\begin{array}{cccccc}
        1 & 0 & 0 & 8 & 3 & 1 \\
        0 & 1 & 0 & 10 & 4 & 1 \\
        0 & 0 & 1 & 7 / 2 & 3 / 2 & 1 / 2
        \end{array}\right] . \quad A^{-1}=\left[\begin{array}{ccc}
        8 & 3 & 1 \\
        10 & 4 & 1 \\
        7 / 2 & 3 / 2 & 1 / 2
        \end{array}\right]
        \end{aligned}
        $$

#### Exercise 4

In this exercise the matrices are all $n \times n$. Each part of the exercise is an implication of the form "If (statement l), then (statement 2)." Mark an implication as True if the truth of (statement 2) always follows whenever ( statement 1) happens to be true. An implication is False if there is an instance in which ( statement 2) is false but (statement l) is true. Justify each answer.

1. If the equation $A \mathbf{x}=\mathbf{0}$ has only the trivial solution, then $A$ is row equivalent to the $n \times n$ identity matrix. (1)
{ .annotate }

    1. True

2. If the columns of $A$ span $\mathbb{R}^n$, then the columns are linearly independent.  (1)
{ .annotate }

    1. True

3. If $A$ is an $n \times n$ matrix, then the equation $A \mathbf{x}=\mathbf{b}$ has at least one solution for each $\mathbf{b}$ in $\mathbb{R}^n$. (1)
{ .annotate }

    1. False

4. If the equation $A \mathbf{x}=\mathbf{0}$ has a nontrivial solution, then $A$ has fewer than $n$ pivot positions. (1)
{ .annotate }

    1. True

5. If $A^T$ is not invertible, then $A$ is not invertibl5.  (1)
{ .annotate }

    1. True

#### Exercise 5
**[Python]** Given

$A=\left[\begin{array}{ccc}1 & 0 & 0 \\ 0 & 3 & 0 \\ 0 & 0 & -3\end{array}\right]$ and $B=\left[\begin{array}{ccc}1 & 1 & 1 \\ 1 & 1 & 1 \\ 1 & 1 & 1\end{array}\right]$.

Solve the matrix equation $X+A=2(X-B)$.

??? answer "&nbsp;"

    The matrix equation $X+A=2(X-B)$ can be rewritten as $X+A=2 X-2 B$. Rearranging terms, we get $X-2 X=-A-2 B$. Simplifying, we have $-X=-A-2 B$. Multiplying by $-1$, we get $X=A+2 B$.

    Substituting the given matrices $A$ and $2B$ into the equation, we have:

    \[
    X=A+2 B=\left[\begin{array}{ccc}
    1 & 0 & 0 \\
    0 & 3 & 0 \\
    0 & 0 & -3
    \end{array}\right]+\left[\begin{array}{lll}
    2 & 2 & 2 \\
    2 & 2 & 2 \\
    2 & 2 & 2
    \end{array}\right]=\left[\begin{array}{ccc}
    3 & 2 & 2 \\
    2 & 5 & 2 \\
    2 & 2 & -1
    \end{array}\right]
    \]

    Therefore, the solution to the matrix equation $X+A=2(X-B)$ is $X=\left[\begin{array}{ccc}3 & 2 & 2 \\ 2 & 5 & 2 \\ 2 & 2 & -1\end{array}\right]$.

#### Exercise 6

**[Python]** Let the matrix $A$ be given by

$A=\left[\begin{array}{cc}
3-2 q & 1 \\
4 & 3+2 q
\end{array}\right]$

where $q$ is a scalar. Calculate $q$ so that

$A^2=\left[\begin{array}{cc}
29 & 6 \\
24 & 125
\end{array}\right]$

??? answer "&nbsp;"

    Let
    $A = \begin{bmatrix} 3 - 2q & 1 \\ 4 & 3 + 2q \end{bmatrix}.$

    Then,
    $A^2 = \begin{bmatrix} (3 - 2q)^2 + 4 & 6 \\ 24 & (3 + 2q)^2 + 4 \end{bmatrix}.$
    Since \( A^2 = \begin{bmatrix} 29 & 6 \\ 24 & 125 \end{bmatrix} \), we have:

    \((3 - 2q)^2 + 4 = 29 \Rightarrow \)  $(3 - 2q)^2 = 25 \Rightarrow 3 - 2q = \pm 5$
    
    **Case 1:** \(3 - 2q = 5 \Rightarrow q = -1\).

    **Case 2:** \(3 - 2q = -5 \Rightarrow q = 4\).

    Check:
    For \(q = -1\), we have:
    $A^2=\left[\begin{array}{ll}5 & 1 \\ 4 & 1\end{array}\right]\left[\begin{array}{ll}5 & 1 \\ 4 & 1\end{array}\right]=\left[\begin{array}{ll}29 & 6 \\ 24 & 9\end{array}\right]$

    For \(q = 4\), we have:
    $A^2=\left[\begin{array}{cc}-5 & 1 \\ 4 & 11\end{array}\right]\left[\begin{array}{cc}-5 & 1 \\ 4 & 11\end{array}\right]=\left[\begin{array}{cc}29 & 6 \\ 24 & 125\end{array}\right]$

    So only \(q = 4\) satisfies the equation.
