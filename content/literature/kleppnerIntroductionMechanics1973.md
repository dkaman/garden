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

    <!--list-separator-->

    -  dot product

        called the _scalar product_ because it represents a way of combining two vectors
        to produce a scalar. \\(\mathbf{A} \cdot \mathbf{B}\\) is defined by:

        \begin{equation}
        \mathbf{A} \cdot \mathbf{B} \equiv \lvert\mathbf{A}\rvert \lvert\mathbf{B}\rvert \cos\theta
        \end{equation}

        where \\(\theta\\) is the angle between \\(\mathbf{A}\\) and \\(\mathbf{B}\\) drawn tail to
        tail.

    <!--list-separator-->

    -  cross product

        two vectors \\(\mathbf{A}\\) and \\(\mathbf{B}\\) forms a third vector \\(\mathbf{C}\\) by:

        \begin{equation}
        \mathbf{C} = \mathbf{A} \times \mathbf{B}
        \end{equation}

        where

        \begin{equation}
        \lvert\mathbf{C}\rvert = \lvert\mathbf{A}\rvert\lvert\mathbf{B}\rvert\sin\theta
        \end{equation}

        in this case \\(\theta\\) is taken as the angle between \\(\mathbf{A}\\) and
        \\(\mathbf{B}\\) and is smaller than \\(\pi\\). the vector product is zero when \\(\theta
        = 0\\) or \\(\theta = \pi\\).

        when \\(\mathbf{A}\\) and \\(\mathbf{B}\\) are drawn tail to tail, they form a plane so
        the direction of \\(\mathbf{C}\\) is perpendicular to that plane.

        {{< figure src="/assets/cross-product.png" >}}

        the vector product is _not_ commutative and so:

        \begin{equation}
        \mathbf{B}\times\mathbf{A} = -\mathbf{A}\times\mathbf{B}
        \end{equation}

        and

        \begin{equation}
        \mathbf{A}\times\mathbf{A} = \mathbf{0}
        \end{equation}


### components of vectors {#components-of-vectors}

the projections of a vector along its coordinate axes are called the
**components** of that vector.

in two dimensions, the components of \\(\mathbf{A}\\) along the \\(\mathit{x}\\) and
\\(\mathit{y}\\) axes are \\(\mathit{A}\_x\\) and \\(\mathit{A}\_y\\).

the magnitube of \\(\mathbf{A}\\) is:

\begin{equation}
\lvert\mathbf{A}\rvert = (\mathit{A}\_x^2 + \mathit{A}\_y^2)^\frac{1}{2}
\end{equation}

and the direction is:

\begin{equation}
\theta = \arctan\frac{\mathit{A}\_y}{\mathit{A}\_x}
\end{equation}

where the angle is measured from the \\(\mathit{x}\\) axis.

vectors can be written entirely by their components, in two dimensions:

\begin{equation}
\mathbf{A} = (\mathit{A}\_x,\mathit{A}\_y)
\end{equation}

and three:

\begin{equation}
\mathbf{A} = (\mathit{A}\_x,\mathit{A}\_y,\mathit{A}\_z)
\end{equation}

thus, all vector operations can be written as equations for components:

\begin{equation}
\mathit{c}\mathbf{A} = (\mathit{c}\mathit{A}\_x,\mathit{c}\mathit{A}\_y)
\end{equation}

the law for vector addition:

\begin{equation}
\mathbf{A} + \mathbf{B} = (\mathit{A}\_x + \mathit{B}\_x,\mathit{A}\_y + \mathit{B}\_y,\mathit{A}\_z + \mathit{B}\_z)
\end{equation}

and dot products:

\begin{equation}
\mathbf{A}\cdot\mathbf{B} = \mathit{A}\_x\mathit{B}\_x + \mathit{A}\_y\mathit{B}\_y + \mathit{A}\_z\mathit{B}\_z
\end{equation}


### base vectors {#base-vectors}

**base vectors** are a set of orthogonal (perpendicular) unit vectors, one for
each dimension.

the unit vector along the \\(\mathit{x}\\) axis is denoted by \\(\mathbf{\hat{i}}\\),
the \\(\mathit{y}\\) axis by \\(\mathbf{\hat{j}}\\) and the \\(\mathit{z}\\) axis by
\\(\mathbf{\hat{k}}\\).
