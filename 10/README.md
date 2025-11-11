<h1 align="center">Differentiation of Simple Functions</h1>

### Session Preparation

Brooks: [Chapter 10](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/RBrooksDK/MSE_book_v2/master/main.pdf)

Some of the exercises may require you to use Python. You may also need to install the `numpy` and `sympy` libraries if you haven't already.

### Resources Danish Class:

[Session notes](https://drive.google.com/file/d/1TBKqEzJ85hpuwXKSoilDalk2qwhHruod/view?usp=sharing)

[Session Resources](https://viaucdk-my.sharepoint.com/:f:/g/personal/rib_viauc_dk/IgCpfSdLLHdeR7pslljlUrhKAXJzbe5-r_AD2M2xDyqvJL8?e=4m0Pmf)

### Exercises

Python solutions will be available after the session.
<!--**[Python]** Means that you are advised to use Python to solve the exercise. You can find the Python solutions [here](https://github.com/RBrooksDK/MSE1_25/blob/main/10/Python_solutions_for_exercises_10.ipynb) or download them [here](Python_solutions_for_exercises_10.ipynb)-->

#### Exercise 1 (Recap)

**[Python]** Given

$A=\left[\begin{array}{ccc}1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9\end{array}\right]$ and $B=\left[\begin{array}{ccc}9 & 8 & 7 \\ 6 & 5 & 4 \\ 3 & 2 & 1\end{array}\right]$.

Solve the matrix equation $X-A=6(X+B)$.

??? answer "&nbsp;"

    $X=\left[\begin{array}{ccc}-11 & -10 & -9 \\ -8 & -7 & -6 \\ -5 & -4 & -3\end{array}\right]$


#### Exercise 2

Find the limits of the following functions:

1. \(\lim\limits_{x \to 0} \frac{x^4-4 x^3+x^2}{x^3+x^2+x}\)
2. \(\lim\limits_{x \to \infty} \frac{x^2+1}{x^2-1}\)
3. \(\lim\limits_{x \to 2} \frac{x-2}{x^2-3 x+2}\)

??? answer "&nbsp;"

    1. \(\lim\limits_{x \to 0} \frac{x^4-4 x^3+x^2}{x^3+x^2+x} = 0\)
    2. \(\lim\limits_{x \to \infty} \frac{x^2+1}{x^2-1} = 1\)
    3. \(\lim\limits_{x \to 2} \frac{x-2}{x^2-3 x+2} = 1\)

#### Exercise 3: Simple Derivatives

Find the derivatives of the following functions:

1. \(f(x)=x^4\)
2. \(f(t)=t^{-\frac{1}{3}}\)
3. \(y=t^{-3.8}\)

??? answer "&nbsp;"

    1. \(f'(x)=4x^3\)
    2. \(f'(t)=-\frac{1}{3}t^{-\frac{4}{3}}\)
    3. \(y'=-3.8t^{-4.8}\)

#### Exercise 4: Derivatives of Powers
Express the following as powers and then differentiate:

1. \(\frac{1}{x^2}\)
2. \(\sqrt[3]{x}\)
3. \(\frac{1}{x \sqrt[4]{x}}\)

??? answer "&nbsp;"

    1. \(\frac{1}{x^2} = x^{-2}\), derivative: \(\frac{d}{dx}x^{-2} = -2x^{-3}\)
    2. \(\sqrt[3]{x} = x^{1/3}\), derivative: \(\frac{d}{dx}x^{1/3} = \frac{1}{3}x^{-2/3}\)
    3. \(\frac{1}{x \sqrt[4]{x}} = x^{-5/4}\), derivative: \(\frac{d}{dx}x^{-5/4} = -\frac{5}{4}x^{-9/4}\)

#### Exercise 5: Derivatives of Sums and Differences

Find the derivatives of the following functions:

1. \(y=2 x^{-7}+\frac{3}{x^2}\)
2. \(f(u)=u^{\frac{5}{3}}-3 u^{-7}\)
3. \(g(z)=8 z^{-2}-\frac{5}{z}\)

??? answer "&nbsp;"

    1. \(\frac{d}{dx}(2 x^{-7}+\frac{3}{x^2}) = -14x^{-8} - 6x^{-3}\)
    2. \(\frac{d}{dx}(u^{\frac{5}{3}}-3 u^{-7}) = \frac{5}{3}u^{2/3} + 21u^{-8}\)
    3. \(\frac{d}{dx}(8 z^{-2}-\frac{5}{z}) = -16z^{-3} + \frac{5}{z^2}\)

#### Exercises 6: Derivatives of Products and Quotients
Use the product rule to differentiate the functions below:  

1. \(f(x)=\left(4 x^3+2\right)(1-3 x)\)
2. \(g(x)=\left(x^2+x+2\right)\left(x^2+1\right)\)
3. \(h(x)=\frac{x^2-1}{x^3+4}\)
4. \(g(t)=\frac{t(t+6)}{t^2+3 t+1}\)

??? answer "&nbsp;"

    1. \(-48x^3 + 12x^2 - 6\)
    2. \( 4x^3 + 3x^2 + 6x + 1\)
    3. \(h^{\prime}(x)=\frac{-x^4+3 x^2+8 x}{\left(x^3+4\right)^2}\)
    4. \(\frac{-3 t^2+2 t+6}{\left(t^2+3 t+1\right)^2}\)


#### Exercise 7: Derivatives using the Chain Rule
1. \((2 x+3)^2\)
2. \(\left(x^2+2 x+1\right)^{12}\)
3. \(f(t)=\sqrt{t^2-5 t+7}\)
4. \(z=\left(x+\frac{1}{x}\right)^{\frac{3}{7}}\)
5. \(\frac{x}{\sqrt{1-x^2}}\)

??? answer "&nbsp;"

    1. \(8 x+12\)
    2. \(12(2 x+2)\left(x^2+2 x+1\right)^{11}\)
    3. \(\frac{2 t-5}{2 \sqrt{t^2-5 t+7}}\)
    4. \(\frac{3}{7}\left(x+\frac{1}{x}\right)^{-4 / 7}\left(1-\frac{1}{x^2}\right)\)
    5. \(\frac{1}{\left(1-x^2\right)^{3 / 2}}\)

#### Exercise 8: Derivatives of Exponential and Logarithmic Functions

1. \(f(x)=\ln \left(2 x^3\right)\)
2. \(f(x)=e^{x^2+x^3}\)
3. \(f(x)=\ln \left(e^x+x^3\right)\)

??? answer "&nbsp;"

    1. \(\frac{3}{x}\)
    2. \(e^{x^2+x^3} (2x+3x^2)\)
    3. \(\frac{e^x+3x^2}{e^x+x^3}\)

#### Exercise 9: Applications of Derivatives

Velocity is the rate of change of position with respect to time. 

Acceleration is the rate of change of velocity with respect to time.

1. Given the position function of a car $s(t) = 5t^2 + 2t + 1$, where $t$ is in seconds and $s(t)$ is in meters, find the velocity function.

    ??? answer "&nbsp;"

        Velocity function: $v(t) = 10t + 2$ m/s        

2. Knowing that acceleration is the derivative of velocity, find the acceleration function.

    ??? answer "&nbsp;"

        Acceleration function: $a(t) = 10$ m/s²

3. Calculate the velocity and acceleration of the car at $t = 3$ seconds.

    ??? answer "&nbsp;"

        Velocity at $t = 3$ seconds: $v(3) = 32$ m/s

        Acceleration at $t = 3$ seconds: $a(3) = 10$ m/s²



