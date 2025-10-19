<h1 align="center">Descriptive Statistics</h1>

### Session Preparation:

Brooks: [Chapter 6](https://drive.google.com/file/d/1P9eidJb5qtlZgvHCtqu4uuPa5FFU0Zpn/view?usp=sharing). You should begin reading before class as it will aid your understanding as the topics get more complex.

### Resources Danish Class:

<<<<<<< HEAD
[Session Resources](https://viaucdk-my.sharepoint.com/:f:/g/personal/rib_viauc_dk/EqVVdPEDkRFImG2F_pAn4C8BaNKeMesysbj3eFJqsKHllw?e=0fiXyu)

--------------------------
=======
[Session notes](https://drive.google.com/file/d/1wAMVD7qDRDlnW3YCHzxZjgo79k14Z6uz/view?usp=sharing)

[Session Resources](https://viaucdk-my.sharepoint.com/:f:/g/personal/rib_viauc_dk/EqVVdPEDkRFImG2F_pAn4C8BaNKeMesysbj3eFJqsKHllw?e=0fiXyu)
>>>>>>> db867ed861d06e3d8a1b5c2a988db954a0d9b752

### Topic Description
Building on our introduction to probability, this session delves deeper into the subject by exploring the concepts of dependent and independent events. We will discuss how the occurrence of one event can affect the probability of another. Conditional probability will be introduced, highlighting how probabilities change when additional information is known. We will also cover the probability of intersections between events, helping to understand overlapping occurrences. Contingency tables will be used to organize data and calculate probabilities effectively, and we will conclude with Bayes' theorem, a powerful tool for updating probabilities based on new evidence.

#### Key Concepts
- Dependent and independent events
- Conditional probability
- The probability for the intersection between events
- Contingency tables
- Bayes' theorem

--------------------------

### Exercises for recitation

Try to do the exercises without using ChatGPT. If you get stuck, you can use ChatGPT to help you along the way. I don't care if you have the correct answers or not; I care that you try to solve the problems - proritise learning over performance, as that will enhance your performance in the long run.

#### Exercise 1: Recap

Let $A$ and $B$ be two events such that:

$$
P(A)=0.3, \quad P(B)=0.2, \quad P(A \cap B)=0.1
$$

Find the probabilities below. State your answers as correct to one decimal place.

a. Find $P(A^c)$. (1)
{ .annotate }

1. $P(A^c)=0.7$.

b. Find $P\left(A \cup B\right)$. (1)
{ .annotate }

1. $P\left(A \cup B\right)=0.4$.

c. Find $P\left(A^c \cap B\right)$. (1)
{ .annotate }

1. $P\left(A^c \cap B\right)=0.1$

d. Find $P\left(A \cap B^c\right)$. (1)
{ .annotate }

1. $P\left(A \cap B^c\right)=0.2$.

e. Find $P\left((A \cup B)^c\right)$. (1)
{ .annotate }

1. $P\left((A \cup B)^c\right)=0.6$.

f. Find $P\left(A^c \cup B\right)$. (1)
{ .annotate }

1. $P\left(A^c \cup B\right)=0.8$.

#### Exercise 2: Rolling Fair Die

I roll a fair die twice and obtain two numbers: $X_1=$ result of the first roll, $X_2=$ result of the second roll.

a. Find the probability that $X_2=4$. (1)
{ .annotate }

1. $\dfrac{1}{6}$

b. Find the probability that $X_1+X_2=7$. (1)
{ .annotate }

1. $\dfrac{1}{6}$

c. Find the probability that $X_1 \neq 2$ and $X_2 \geq 4$. (1)
{ .annotate }

1. $\dfrac{5}{12}$

#### Exercise 3: Venn and Probability

Let $A, B$, and $C$ be three events with probabilities given:

<img src="src/venn1.png" width = "200">

Find the probabilities below. State you answers as irreducible fractions.

a. $P(A \mid B)$ (1)
{ .annotate }

1. $\dfrac{4}{7}$

b. $P(C \mid B)$ (1)
{ .annotate }

1. $\dfrac{3}{7}$

c. $P(B \mid A \cup C)$ (1)
{ .annotate }

1. $\dfrac{5}{14}$

d. $P(B \mid (A, C))$ (1)
{ .annotate }

1. $\dfrac{1}{2}$

#### Exercise 4: More Planes
The probability that a regularly scheduled flight departs on time is $0.83$; the probability that it arrives on time is $0.82$; and the probability that it departs and arrives on time is $0.78$. Find the probability that a plane. State your answers as correct to four decimal places.

a. Arrives on time, given that it departed on time (1)
{ .annotate }

1. 0.9398

b. Departed on time, given that it has arrived on time (1)
{ .annotate }

1. 0.9512

c. Arrives on time, given that it did not depart on time (1)
{ .annotate }

1. 0.2353

</details>
<br>

#### Exercises 5: Independence and Contingency Tables
A survey was conducted to determine the employment rate of recently graduated engineering students. The survey was conducted one year after graduation and was made for ICT Engineers, Civil Engineers, Mechanical Engineers, and Global Business Engineers. The graduates were classified in one of two employment categories: (1) employed/studying and (2) unemployed. 40% of the respondents had studied ICT Engineering and of these 85% were employed/studying. Of all the respondents, 20% were unemployed. Of the 100 former civil engineering students who took part in the survey, 20% were unemployed. The proportion of unemployed Mechanical and Civil engineering students was the same and the survey included exactly 9 unemployed mechanical engineering students. 300 students took part in the survey.

<<<<<<< HEAD
a. Based on this information, construct a 2 x 4 contingency table for the survey results.
=======
        - Within 1 standard deviation (17.37 to 29.82): 91.23%
        - Within 2 standard deviations (11.15 to 36.05): 96.49%
        - Within 3 standard deviations (4.92 to 42.27): 96.49%

        The data does not perfectly follow the Empirical Rule, indicating it may not be normally distributed.
    
9. Inspect the histogram for skewness. (1)
{ .annotate }

    1. The histogram shows a right (positive) skew, with a longer tail on the right side.

#### Exercise 5: Box Plot (Python)

A factory fills 1kg bags of sugar. The weights of a sample of 20 bags are recorded below (in kg):

{1.00, 1.01, 1.05, 0.99, 0.97, 1.01, 0.98, 0.99, 1.06, 1.06, 0.96, 1.00, 1.03, 0.97, 1.00, 0.99, 1.08, 1.01, 1.32, 0.82, 0.86}

The following box plot represents the distribution of the weights:

![Box Plot](src/Ex05.png)

1. Identify the median weight from the box plot. (1)
{ .annotate }

    1. Median ≈ 1.00 kg

2. Estimate the first (Q1) and third (Q3) quartiles. (1)
{ .annotate }

    1. Q1 ≈ 0.98 kg, Q3 ≈ 1.03 kg

3. Calculate the interquartile range (IQR). (1)
{ .annotate }

    1. IQR ≈ 0.05 kg

4. Determine the range of weights. (1)
{ .annotate }

    1. Range ≈ 0.5 kg

5. Explain what the outliers represent in this context.

    ??? answer "&nbsp;"

        The outliers represent bags that are significantly underfilled or overfilled compared to the majority of bags.

6. What could the outliers indicate about the factory's filling process?

    ??? answer "&nbsp;"

        The outliers could indicate inconsistencies in the filling process, such as equipment malfunctions or human error. They do not suggest inaccuaracy of the scale, rather issues in the filling process itself.

7. Based on the box plot, discuss the symmetry or skewness of the weight distribution. (1)
{ .annotate }

    1. The box plot appears slightly right skewed.

8. Based on the determined skewness, discuss the values of mean, mode, and median. (1)
{ .annotate }

    1. In a right-skewed distribution, the mean is typically greater than the median, which is greater than the mode.

#### Exercise 6: Empirical Rule (Python)

For each dataset below, determine whether the data appear approximately normal, or not.

Use the Empirical Rule (68.3–95.4–99.7%) to justify your answer.

1. Response Times (ms) - Mean = 300, SD = 50, within 1 SD: 55%, within 2 SD: 78%, within 3 SD: 90% (1)
{ .annotate }

    1. Not Normal

2. Bug Reports per Week - Mean = 12, SD = 4, within 1 SD: 68%, within 2 SD: 94%, within 3 SD: 99% (1)
{ .annotate }

    1. Approximately Normal

3. Exam Scores: {55, 60, 62, 65, 68, 70, 72, 75, 78, 80, 82, 85, 88, 90, 92, 95} (1)
{ .annotate }

    1. Approximately Normal

4. Daily Step Counts (in thousands): {3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15} (1)
{ .annotate }

    1. Not Normal

### Challenge Exercises

#### Challenge 1: The “German Tank” Problem (Build Numbers)

A military intelligence unit intercepts serial numbers from enemy tanks. The numbers are sequential from 1 to an unknown maximum \(N\). In one skirmish they observe (unordered):
\(\{12, 38, 71, 5, 44, 73, 29, 55\}\).

Let \(n\) be the sample size and \(m\) the maximum observed number. Compute \(n\) and \(m\). (1)  
{ .annotate }

1. \(n=8,\ m=73\)

Two estimators for \(N\):  

MLE: \(\hat N_{\text{MLE}} = m\)  

Unbiased: \(\hat N_{\text{U}} = m\cdot\frac{n+1}{n}-1\)  

Compute both and give an integer estimate.
>>>>>>> db867ed861d06e3d8a1b5c2a988db954a0d9b752

??? answer "&nbsp;"
    <img src="src/contingency.png" width = "300">

    Technically, the sums and totals are not part of the contingency tables. They are added to make it easier to calculate the probabilities.


b. What is the probability that an unemployed respondent is a former ICT student? State your answer as an irreducible fraction. (1)
{ .annotate }

1. $\dfrac{3}{10}$

c. If a respondent is unemployed, what is the probability that the respondent was a GBE student? State your answer as an irreducible fraction. (1)
{ .annotate }

1. $\dfrac{13}{60}$

d. Is being unemployed independent from being a former ICT student? (1)
{ .annotate }

??? answer "&nbsp;"
    You can compare any a priori probability with the corresponding a posteriori probability. E.g. you found an aposteriori probability of $\dfrac{3}{10}$ in (b). The a priori probability is $\dfrac{2}{5}$. Since the two probabilities are not equal, the two events are dependent:

    $P(\text{ICT} \mid \text{Unemployed}) = \dfrac{3}{10} \neq \dfrac{2}{5} = P(\text{ICT})$

#### Exercise 6: Bayes' Theorem
Disease $A$ occurs with probability 0.1, and disease $B$ occurs with probability 0.2. It is not possible to have both diseases. You have a single test. This test reports positive with probability 0.8 for a patient with disease $A$, with probability 0.5 for a patient with disease $B$, and with probability 0.01 for a patient with no disease - call the latter event $W$. Stating your answer as correct to four decimal places, if the test comes back positive, what is the probability you have either:

a. Disease $A$

b. Disease $B$ or

c. No disease

Note: You need to calculate three probabilities; one for each of the three events stated in a-c.

??? answer "&nbsp;"
    a. Disease $A$: 0.4278

    b. Disease $B$: 0.5348

    c. No disease: 0.0374

#### Exercise 7: Challenge Exercise
Only use time on this exercise if you have time left after completing the other exercises and you found them too easy. The problem is taken from the exam in Stochastic Modelling and Processes (IT-SMP1) on the 6th/7th semester.

You choose a point $(A, B)$ uniformly at random in the unit square $\{(x, y): 0 \leq x, y \leq 1\}.

<p align="center">
    <img src="src/challenge.png" width="200">
</p>

What is the probability that the equation

$$
A X^2+X+B=0
$$

has real solutions?

[solution](Solution7.pdf)

### Additional Solutions
[Some Python Solutions](https://github.com/RBrooksDK/MSE1/blob/main/06_Conditional_Probability_and_Bayes_Theorem/some_solutions.ipynb)

[Solutions made in class](https://drive.google.com/open?id=1lCgiFIzOLAuDSEQjUyeZiyWsWt63Ex8d&usp=drive_fs)