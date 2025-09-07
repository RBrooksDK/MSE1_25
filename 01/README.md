---
tags:
    - Introduction
    - Arithmetic Rules
    - Powers
    - Roots
    - Exponents
    - Logarithms
    - Functions
    - Domain
    - Range
    - Inverse Functions
    - Composite Functions
---

<h1 align="center">Basic Arithmetic and Functions</h1>
In this introductory session, we lay the foundation for the mathematics used in software development. We begin with an overview of the course structure, learning objectives, and expectations. Then, we focus on key arithmetic rules and the fundamental properties of functions, which form the basis for the more advanced topics covered later in the course.

The session includes understanding and applying rules of powers, roots, exponents, and logarithms. We also explore the definition of functions as well as their domains and ranges. Finally, we introduce the concepts of inverse and composite functions, which are essential for further work in the course. Special emphasis is placed on logarithms and their applications in software development, as they play a central role in many algorithms and data processing methods.

<hr/>

### Session Preparation:

Brooks: [Chapter 1](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/RBrooksDK/MSE_book_v2/master/main.pdf).

### Resources Danish Class
[Lecture notes](https://drive.google.com/file/d/1b4RxsUGG_Mwa5OHSsLZ1Xymlc0V2cLcc/view?usp=sharing)

[Session materials](https://viaucdk-my.sharepoint.com/:f:/g/personal/rib_viauc_dk/EtdW6vDKB6FHsPZdtO6XUhMB5n3uwC00IoyfXj5g1O6JlA?e=HPKxg0)

<hr/>

### Exercises

#### Exercise 1:

Solve the following equations:

1. $\ 2-\frac{4 x+3}{x+x^2}=\frac{2 x}{x+1}-\frac{5}{x}$
2. $\ -2+2 \ln 3 x=17$
3. $\ \ln (x+1)^2=2$
4. $\ \ln \left(x^2+1\right)=8$
5. $\ 5^{3 x+2}=25^{x-1}$
6. $\ 2^{x+1}=4^{x-2}$

??? answer "&nbsp;"

    1. $x = -\frac{2}{3}$
    2. $x = \frac{e^{\frac{19}{2}}}{3}$
    3. $x = -1 \pm e$
    4. $x = \pm \sqrt{e^8 - 1}$
    5. $x = -4$
    6. $x = 5$

#### Exercise 2:

According to Einstein's theory of relativity, the mass of a particle is given by:

$$
m=\frac{m_0}{\sqrt{1-\left(\frac{v}{c}\right)^2}}
$$

where
$m_0$ is the rest mass of the particle,
$v$ is the velocity of the particle, and
$c$ is the speed of light in a vacuum.

1. Make $v$ the subject of the formula given $v>0$.

    ??? answer "&nbsp;"

        $v=c \cdot \sqrt{1-\left(\frac{m_0}{m}\right)^2}$

2. Find the velocity required to increase the mass of a particle to three times its rest mass. Provide the value for $v$ as a fraction of $c$ (or as a decimal).

    ??? answer "&nbsp;"

        $v=0.943 c$

#### Exercise 3
Determine the domain and range for each of the real functions below. It is a good idea to plot the functions using software (e.g., Geogebra, WolframAlpha, etc.):

1. $\ f(x)=\frac{1}{x-7}$

    ??? answer "&nbsp;"

        Domain: $\mathbb{R} \backslash\{7\}$;

        Range: $\mathbb{R} \backslash\{0\}$

2. $\ f(x)=\sqrt{x+3}$

    ??? answer "&nbsp;"

        Domain: $\mathbb{R}_ {\geq-3}$;

        Range: $\mathbb{R}_ {\geq 0}$

#### Exercise 4
Find each of the following composite functions:

1. $\ g \circ f$ when $f(x)=3 x+1$ and $g(x)=x^2$.

    ??? answer "&nbsp;"

        $(g \circ f)(x)=9 x^2+1+6 x$

2. $f \circ g$ when $f(x)=x^2+1$ and $g(x)=\frac{1}{x}$.

    ??? answer "&nbsp;"

        $(f \circ g)(x)=\frac{1}{x^2}+1$

3. $\ g \circ f$ when $f$ and $g$ are defined as in part b.

    ??? answer "&nbsp;"

        $(g \circ f)(x)=\frac{1}{x^2+1}$

#### Exercise 5
Find the inverse function:

1. $\ f(x)=\frac{6}{5-x}$

    ??? answer "&nbsp;"

        $f^{-1}(x)=5-\frac{6}{x}$

2. $\ f(x)=-\ln (1-2 x)+1$

    ??? answer "&nbsp;"

        $f^{-1}(x)=\left(1-e^{1-x}\right) / 2$

3. $\ f(x)=2 \cdot 10^{3 x}-1$

    ??? answer "&nbsp;"

        $f^{-1}(x)=\frac{\log \left(\frac{x+1}{2}\right)}{3}$

#### Exercise 6

A bacterial culture starts with 1000 bacteria at time $t=0$, and the number doubles every 40 minutes.

1. Find a functional expression for the number of bacteria at time $t$ (measured in minutes).

    ??? answer "&nbsp;"

        $f(t)=1000 \cdot 2^{t / 40}$

2. Find the number of bacteria after one hour.

    ??? answer "&nbsp;"

        $f(60) \approx 2828$

3. After how many minutes will there be 50000 bacteria?

    ??? answer "&nbsp;"

        approx. 225.75 minutes

#### Exercise 7

Determine whether the given function is invertible by checking if it is injective (one-to-one) and surjective (onto). If you conclude that the function is invertible, determine it's inverse function.

1. $f: R \backslash\{1\} \rightarrow R \backslash\{0\}, f(x)=\frac{2}{x-1}$

    ??? answer "&nbsp;"

        The function is invertible.

        $f^{-1}(x)=\frac{2}{x}+1$

2. $f: R \backslash\{3\} \rightarrow R, f(x)=\frac{x+1}{x-3}$

    ??? answer "&nbsp;"

        The function is not surjective, thus it is not invertible.

3. $f: R \rightarrow R, f(x)=x^3-3 x$

    ??? answer "&nbsp;"

        The function is not injective, thus it is not invertible.

### Challenge Exercises

Some second order polynomials do not have any roots among the real numbers. For example, no real value of $x$ fulfills the equation $x^2+1=0$. However, if we define the imaginary number $i=\sqrt{-1}$, it is seen than the equation is true for $x= \pm i$ :

$$
i^2+1=-1+1=0 \quad \text { and } \quad(-i)^2+1=-1+1=0
$$

#### Challenge Exercise 1

Solve the equations below (a second order equation with imaginary roots is solved the same way you would solve a regular second order equation.):

1. $9 x^2+64=0$

    ??? answer "&nbsp;"

        $x= \pm \frac{8}{3} i$

2. $x^2+10 x+169=0$

    ??? answer "&nbsp;"

        $x=-5 \pm 12 i$

3. $6 x^2+13 ix-2=0$

    ??? answer "&nbsp;"

        $x=-\frac{1}{6} i$ or $x=-2 i$

#### Challenge Exercise 2

Show that the value of each of the expressions below is real (i.e. does not contain $i$ ):

1. $(1+i)(1-i)$

    ??? answer "&nbsp;"

        $(1+i)(1-i)=2$

2. $(a+b i)(a-b i)$

    ??? answer "&nbsp;"

        $(a+b i)(a-b i)=a^2-b^2 i^2=a^2+b^2$

#### Challenge Exercise 3

Calculate or reduce each of the expression below:

1. $i^{2017}$

    ??? answer "&nbsp;"

        $i$

2. $\frac{1}{2+3 i}+\frac{1}{2-3 i}$

    ??? answer "&nbsp;"

        $\frac{4}{13}$

3. $\frac{1+i}{1-i}$

    ??? answer "&nbsp;"

        $i$