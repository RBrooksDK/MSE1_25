<h1 align="center">Gradients and Partial Derivatives</h1>

### Session Preparation:

Brooks: [Section 10.5. + Chapter 11](https://drive.google.com/file/d/1P9eidJb5qtlZgvHCtqu4uuPa5FFU0Zpn/view?usp=sharing). You should begin reading before class as it will aid your understanding as the topics get more complex

### Resources Danish Class:

[Session notes](https://drive.google.com/file/d/1TBKqEzJ85hpuwXKSoilDalk2qwhHruod/view?usp=sharing)

[Session Resources](https://viaucdk-my.sharepoint.com/:f:/g/personal/rib_viauc_dk/IgCpfSdLLHdeR7pslljlUrhKAXJzbe5-r_AD2M2xDyqvJL8?e=4m0Pmf)


### Exercises

#### Exercise 1 (recap): Derivatives

Find the derivatives of the following functions:

1. \(\frac{1}{\left(1+e^{2 x}\right)^3}\)
2. \((2 x+5)^7\left(3 x^4-8\right)^5\)

??? answer "&nbsp;"

    1. \(-\frac{6 e^{2 x}}{\left(1+e^{2 x}\right)^4}\)

    2. \(14(2 x+5)^6\left(3 x^4-8\right)^5+60 x^3(2 x+5)^7\left(3 x^4-8\right)^4\)

#### Exercise 2: Second Order Derivative Test

For the following, find all stationary points, find the second order derivative at these points, and classify them as a maximum or minimum using the second order derivative test.

1. \(f(x)=6 x-x^2\)
2. \(f(x)=-(x-5)^2\)

??? answer "&nbsp;"

    1. Maximum at \(x=3\) since \(f^{\prime \prime}(3) < 0\)
    2. Maximum at \(x=5\) since \(f^{\prime \prime}(5) < 0\)

#### Exercise 3: Stationary Points

Find all stationary points (maxima, minima, or inflection points), and intervals of concavity for the following function:

$$
f(x)=x^3-12 x
$$

??? answer "&nbsp;"

    \(\begin{aligned} & 3 x^2-12=0 \Rightarrow x= \pm 2 \\ & f^{\prime \prime}(-2)=-12 \Rightarrow \text { local max local max of } 16 \text { at } x=-2 \\ & f^{\prime \prime}(2)=12 \Rightarrow \text { local min local min of }-16 \text { at } x=2\end{aligned}\)

    

#### Exercise 4: Functions of Two Variables

Find the domain and range of the function \(f(x, y)=\sqrt{36-9 x^2-9 y^2}\) and sketch the domain.


??? answer "&nbsp;"

    Domain: \(\left\{(x, y) \in \mathbb{R}^2 \mid x^2+y^2 \leq 4\right\}\)

    Range: \([0, 6]\)

#### Exercise 5: Partial Derivatives
Calculate \(\partial f / \partial x\) and \(\partial f / \partial y\) for the following functions:

1. \(f(x, y)=x^2-3 x y+2 y^2-4 x+5 y-12\)
2. \(f(x, y)=x^2 y^3-2 x^3 y^2+3 x y-4\)

??? answer "&nbsp;"

    1. \(\partial f / \partial x = 2x-3y-4\) and \(\partial f / \partial y = -3x+4y+5\)
    2. \(\partial f / \partial x = 2xy^3-6x^2y^2+3y\) and \(\partial f / \partial y = 3x^2y^2-4x^3y+3x\)

#### Exercise 6: Gradients

Let

$$
f(x, y)=x^2+4 y^2-3 x y .
$$

1. Compute the gradient \(\nabla f(x, y)\).
2. Evaluate the gradient at the point ( 1,2 ).
3. Explain what the gradient vector at that point tells you about the behaviour of the function.

??? answer "&nbsp;"
    1. \(\nabla f(x, y)=\langle 2x-3y,\ 8y-3x\rangle = \begin{bmatrix} 2x-3y \\ 8y-3x \end{bmatrix}\)
    2. \(\nabla f(1,2)=\begin{bmatrix} 2(1)-3(2) \\ 8(2)-3(1) \end{bmatrix}=\begin{bmatrix} -4 \\ 13 \end{bmatrix}\)
    3. The gradient vector points in the direction in which the function \(f(x, y)\) increases most rapidly. From the point (1, 2) in the \(x y\)-plane, moving in the direction of the vector \((-4,13)\) will result in the steepest increase in the value of the function.