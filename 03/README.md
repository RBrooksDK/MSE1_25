---
tags:
    - Sets
    - Set Theory
    - Sets and Subsets
    - Power Set
    - Cardinality
    - Union
    - Intersection
    - Complement
    - Set Difference
    - Symmetric Difference
    - De Morgan’s Laws
    - Set Identities
    - Membership Tables
    - Cartesian Product
    - Tuples
    - Bitsets   
---

<h1 align="center">Set Theory</h1>

In this session, we cover the basics of set theory, including different ways to describe sets, fundamental set operations, and important properties and laws governing sets. 

<hr/>

### Session Preparation:

Brooks: [Chapter 3](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/RBrooksDK/MSE_book_v2/master/main.pdf).

### Resources Danish Class:

[Session notes]()

[Session Resources]()

<hr/>

### Exercises

#### Exercise 1: Roster vs. Set-Builder (equivalence)

For each pair, decide whether the two notations define the **same** set.

1. \(A=\{2,4,6,8\}\) and \(A=\{\,x\in\mathbb Z\mid 1\le x\le 8,\; x\text{ even}\,\}\). (1)
{ .annotate }

    1. Same.

2. \(B=\{a,e,i,o,u\}\) and \(B=\{\,l\mid l\text{ is a vowel in English}\,\}\). (1)
{ .annotate }

    1. Same.

3. \(C=\{x\in\mathbb Z\mid x^2<10\}\) and \(C=\{-3,-2,-1,0,1,2,3\}\). (1)
{ .annotate }

    1. Same.

#### Exercise 2: Membership \(\in\) / \(\notin\)

Let \(U=\mathbb Z\), \(E=\{x\in\mathbb Z\mid x\equiv 0\pmod 2\}\), \(O=U\setminus E\).

1. Decide: \( -7\in E\ ?\) (1)
{ .annotate }

    1. No, \(-7\in O\).

2. Decide: \(0\in E\ ?\) (1)
{ .annotate }

    1. Yes.

3. Decide: \( \pi\in U\ ?\) (1)
{ .annotate }

    1. No, \(\pi\notin\mathbb Z\).

#### Exercise 3: Subset vs. Proper Subset

Let \(A=\{1,2\}\), \(B=\{1,2,3\}\), \(C=\{1,2\}\).

1. Is \(A\subseteq B\)? Is \(A\subset B\)? (1)
{ .annotate }

    1. Yes; Yes (proper).

2. Is \(A\subseteq C\)? Is \(A\subset C\)? (1)
{ .annotate }

    1. Yes; No (equal, not proper).

3. Give an example of two **disjoint** nonempty subsets of \(\{1,2,3,4\}\). (1)
{ .annotate }

    1. \(\{1,3\}\) and \(\{2,4\}\).

#### Exercise 4: Cardinality and Power Set

1. Compute \(|\mathcal P(\{a,b,c\})|\) and list \(\mathcal P\).

    ??? answer "&nbsp;"

        \(2^3=8\). \(\{\emptyset,\{a\},\{b\},\{c\},\{a,b\},\{a,c\},\{b,c\},\{a,b,c\}\}\).

2. For \(S=\{1,2,3,4,5\}\), how many subsets contain the element \(1\)?

    ??? answer "&nbsp;"

        \(2^{4}=16\) (choose freely among the other 4).

#### Exercise 5: Core Operations (compute explicitly)

Let \(U=\{1,2,\dots,10\}\), \(A=\{1,3,4,8,10\}\), \(B=\{2,3,7,8\}\).

1. \(A\cup B\) (1)
{ .annotate }

    1. \(\{1,2,3,4,7,8,10\}\).

2. \(A\cap B\) (1)
{ .annotate }

    1. \(\{3,8\}\).

3. \(A\setminus B\) and \(B\setminus A\) (1)
{ .annotate }

    1. \(A\setminus B=\{1,4,10\}\), \(B\setminus A=\{2,7\}\).

4. \(A^\mathrm c\) (complement in \(U\)) (1)
{ .annotate }

    1. \(\{2,5,6,7,9\}\).

5. \(A\oplus B\) (symmetric difference) (1)
{ .annotate }

    1. \(\{1,2,4,7,10\}\).

#### Exercise 6: Interval Notation (translation)

Translate between set-builder and interval notation in \(\mathbb R\).

1. \(\{x\in\mathbb R\mid -2\le x<3\}\) (1)
{ .annotate }

    1. \([-2,3)\).

2. \((-∞,0]\cup(5,∞)\) in builder form. (1)
{ .annotate }

    1. \(\{x\in\mathbb R\mid x\le 0\ \text{or}\ x>5\}\).

#### Exercise 7: Set Operations and Cardinality

Consider the sets $A=\{e, f, g\}$ and $B=\{a, e, g, h\}$. Determine each set and its cardinality:

1. $A \cup B$ and $|A \cup B|$ (1)
{ .annotate }

    1. $\{a, e, f, g, h\}$ and $5$.

2. $A \cap B$ and $|A \cap B|$ (1)
{ .annotate }

    1. $\{e, g\}$ and $2$.

3. $B-A$ and $|B-A|$ (1)
{ .annotate }

    1. $\{a, h\}$ and $2$.

4. $A-B$ and $|A-B|$ (1)
{ .annotate }

    1. $\{f\}$ and $1$.

#### Exercise 8: Set Identities

1. Prove that \(A \cup (A \cap B) = A\) using fundamental set identities.

    ??? answer "&nbsp;"

        \[
        \begin{aligned}
        A \cup (A \cap B)
          &= (A \cup A)\,\cap\,(A \cup B) && \text{distributivity}\\
          &= A \cap (A \cup B)            && \text{idempotence}\\
          &= A                             && \text{absorption.}
        \end{aligned}
        \]

2. Prove that \(\left(A \cap A^{c}\right) \cup (A \cap B) \cup \left(A^{c} \cap B\right) = B\) using set identities.

    ??? answer "&nbsp;"

        \[
        \begin{aligned}
        (A \cap A^c) \cup (A \cap B) \cup (A^c \cap B)
          &= \varnothing \cup \big[(A \cap B) \cup (A^c \cap B)\big] && A \cap A^c=\varnothing \\
          &= B \cap (A \cup A^c)                                    && \text{distributivity}\\
          &= B \cap U                                               && \text{complement law}\\
          &= B.                                                     && \text{identity}
        \end{aligned}
        \]

3. Prove that \(\big((A^c \cup B)^c\big) \cup A = A\) using set identities.

    ??? answer "&nbsp;"

        \[
        \begin{aligned}
        \big((A^c \cup B)^c\big) \cup A
          &= \big((A^c)^c \cap B^c\big) \cup A && \text{De Morgan}\\
          &= (A \cap B^c) \cup A               && \text{double complement}\\
          &= A \cup (A \cap B^c)               \\
          &= A.                                 && \text{absorption}
        \end{aligned}
        \]

4. Determine if \((A \oplus B) \cup A = A \cup B\) using set identities.

    ??? answer "&nbsp;"

        \[
        \begin{aligned}
        (A \oplus B) \cup A
          &= \big((A \cap B^c) \cup (A^c \cap B)\big) \cup A && \text{def.\ of }\oplus\\
          &= \big(A \cap B^c\big) \cup A \cup \big(A^c \cap B\big)\\
          &= A \cup \big(A^c \cap B\big)                    && A \cup (A \cap X)=A\\
          &= (A \cup A^c)\cap (A \cup B)                    && \text{distributivity}\\
          &= U \cap (A \cup B)\\
          &= A \cup B.
        \end{aligned}
        \]
