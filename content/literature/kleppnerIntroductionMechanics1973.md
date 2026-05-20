---
title: "An Introduction to Mechanics"
author: ["Daniel Kleppner", "Robert J. Kolenkow"]
tags: ["physics"]
draft: false
---

Kleppner, Daniel, and Robert Kolenkow. <i>An Introduction to Mechanics</i>. 1st ed., McGraw Hill, 1973.

this is the primary text for [mit ocw 8.012 - physics I - classical mechanics]({{< relref "20260516223414-mit_ocw_8_012_physics_i_classical_mechanics.md" >}})


## chapter 1: vectors and kinematics - a few mathematical preliminaries {#chapter-1-vectors-and-kinematics-a-few-mathematical-preliminaries}


### vectors {#vectors}

vectors notation allows for physical laws to be written in compact form

for example, newton's second law can be written

\\[

\begin{aligned}
F\_x &= ma\_x \\\\
F\_y &= ma\_y \\\\
F\_z &= ma\_z
\end{aligned}

\\]

but in vector notation, it is written:

\begin{equation}
\mathbf{F} = m\mathbf{a}
\end{equation}


#### definition of a vector {#definition-of-a-vector}

3 points of view: geometric, analytic, and axiomatic, but for physics it's
sufficient to use geometric and analytic.

to describe a vector, its length and direction must be specified. unless
specified, parallel translation does not change a vector, and vectors that have
the same length and direction are equal.

the length of a vector is called its **magnitude** which is indicated by vertical
bars, for example the magnitude of \\(\mathbf{A}\\) is written as
\\(\lvert\mathbf{A}\rvert\\).

if the length of a vector is one unit, it is called a **unit vector** and is
labeled with a caret, like \\(\mathbf{\hat{A}}\\).

it follows that:

\begin{equation}
\mathbf{\hat{A}} = \frac{\mathbf{A}}{\lvert\mathbf{A}\rvert}
\end{equation}

and conversely:

\begin{equation}
\mathbf{A} = \lvert\mathbf{A}\rvert\hat{\mathbf{A}}
\end{equation}


#### the algebra of vectors {#the-algebra-of-vectors}

<!--list-separator-->

-  the multiplication of a vector by a scalar

    multiplication of vector \\(\mathbf{A}\\) by a positive scalar \\(\mathit{b}\\) then we
    get a new vector \\(\mathbf{C}\\)

    \begin{equation}
    \mathbf{C} = \mathit{b}\mathbf{A}
    \end{equation}

    in this situation \\(\hat{\mathbf{C}} = \hat{\mathbf{A}}\\) and
    \\(\lvert\mathbf{C}\rvert = \mathit{b}\lvert\mathbf{A}\rvert\\)

    multiplying a vector by \\(-1\\) creates a new vector with opposite direction; a
    negative scalar can change both magnitude and direction.

<!--list-separator-->

-  addition of two vectors

    to add \\(\mathbf{B}\\) to \\(\mathbf{A}\\), place the tail of \\(\mathbf{B}\\) at the head
    of \\(\mathbf{A}\\), and the sum is the vector from the tail of \\(\mathbf{A}\\) to the
    head of \\(\mathbf{B}\\), like:

    {{< figure src="/assets/vector-addition.png" >}}

    since \\(\mathbf{A} - \mathbf{B} = \mathbf{A} + (-\mathbf{B})\\), in order to
    subtract \\(\mathbf{B}\\) from \\(\mathbf{A}\\), we can just multiply \\(\mathbf{B}\\) by
    \\(-1\\) and then add, like:

    {{< figure src="/assets/vector-subtraction.png" >}}

    this can also be constructed by placing the _head_ of \\(\mathbf{B}\\) at the _head_
    of \\(\mathbf{A}\\), then \\(\mathbf{A} - \mathbf{B}\\) is drawn from the tail of
    \\(\mathbf{A}\\) to the tail of \\(\mathbf{B}\\).

    **commutative law**:
    \\[

    \begin{aligned}
    \mathbf{A} + \mathbf{B} = \mathbf{B} + \mathbf{A}
    \end{aligned}

    \\]

    **associative law**:
    \\[

    \begin{aligned}
    \mathbf{A} + (\mathbf{B} + \mathbf{C}) &= (\mathbf{A} + \mathbf{B}) + \mathbf{C} \\\\
    \mathit{c}(\mathit{d}\mathbf{A}) &= (\mathit{c}\mathit{d})\mathbf{A}
    \end{aligned}

    \\]

    **distributive law**:
    \\[

    \begin{aligned}
    (\mathit{c} + \mathit{d})\mathbf{A} &= \mathit{c}\mathbf{A} + \mathit{d}\mathbf{A} \\\\
    \mathit{c}(\mathbf{A} + \mathbf{B}) &= \mathit{c}\mathbf{A} + \mathit{c}\mathbf{B}
    \end{aligned}

    \\]

<!--list-separator-->

-  products of two vectors

    there are two kinds of vector products, the scalar product or **"dot" product**, and
    the vector product or **"cross" product**.
