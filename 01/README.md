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

### Session Preparation:

Brooks: [Chapter 1](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/RBrooksDK/MSE_book_v2/master/main.pdf).

### Resources

[Lecture notes]()

[Session materials]()

In this introductory session, we lay the foundation for the mathematics used in software development. We begin with an overview of the course structure, learning objectives, and expectations. Then, we focus on key arithmetic rules and the fundamental properties of functions, which form the basis for the more advanced topics covered later in the course.

The session includes understanding and applying rules of powers, roots, exponents, and logarithms. We also explore the definition of functions as well as their domains and ranges. Finally, we introduce the concepts of inverse and composite functions, which are essential for further work in the course. Special emphasis is placed on logarithms and their applications in software development, as they play a central role in many algorithms and data processing methods.

### Exercises

<style>
body[data-md-color-scheme] .md-content ol       { list-style-type: lower-alpha; }
body[data-md-color-scheme] .md-content ol li    { padding-left: 10px; }
</style>

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

3. $\ g \circ f$ when $f$ and $g$ are defined as in exercise (2).

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