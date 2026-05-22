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

properties of base vectors:

\\[

\begin{aligned}
\mathbf{\hat{i}}\cdot\mathbf{\hat{i}} &= \mathbf{\hat{j}}\cdot\mathbf{\hat{j}} = \mathbf{\hat{k}}\cdot\mathbf{\hat{k}} = 1 \\\\
\mathbf{\hat{i}}\cdot\mathbf{\hat{j}} &= \mathbf{\hat{j}}\cdot\mathbf{\hat{k}} = \mathbf{\hat{k}}\cdot\mathbf{\hat{i}} = 0 \\\\
\mathbf{\hat{i}}\times\mathbf{\hat{j}} &= \mathbf{\hat{k}} \\\\
\mathbf{\hat{j}}\times\mathbf{\hat{k}} &= \mathbf{\hat{i}} \\\\
\mathbf{\hat{k}}\times\mathbf{\hat{i}} &= \mathbf{\hat{j}}
\end{aligned}

\\]

any vector can be  written in terms of these base vectors:

\begin{equation}
\mathbf{A} = \mathit{A}\_x\mathbf{\hat{i}} + \mathit{A}\_y\mathbf{\hat{j}} + \mathit{A}\_z\mathbf{\hat{k}}
\end{equation}

{{< figure src="/assets/base-vector-example.png" >}}

to compute the cross product of vectors using base vectors:

\begin{equation}
\mathbf{A}\times\mathbf{B} = (\mathit{A}\_x\mathbf{\hat{i}} + \mathit{A}\_y\mathbf{\hat{j}} + \mathit{A}\_z\mathbf{\hat{k}}) \times (\mathit{B}\_x\mathbf{\hat{i}} + \mathit{B}\_y\mathbf{\hat{j}} + \mathit{B}\_z\mathbf{\hat{k}})
\end{equation}

considering the first term gives us:

\begin{equation}
\mathit{A}\_x\mathbf{\hat{i}}\times\mathbf{B} = \mathit{A}\_x\mathit{B}\_x(\mathbf{\hat{i}}\times\mathbf{\hat{i}}) + \mathit{A}\_x\mathit{B}\_y(\mathbf{\hat{i}}\times\mathbf{\hat{j}}) + \mathit{A}\_x\mathit{B}\_z(\mathbf{\hat{i}}\times\mathbf{\hat{k}})
\end{equation}

because \\(\mathbf{\hat{i}}\times\mathbf{\hat{i}} = 0\\), \\(\mathbf{\hat{i}}\times\mathbf{\hat{j}} = \mathbf{\hat{k}}\\), and \\(\mathbf{\hat{i}}\times\mathbf{\hat{k}} = -\mathbf{\hat{j}}\\), this gives:

\begin{equation}
\mathit{A}\_x\mathbf{\hat{i}}\times\mathbf{B} = \mathit{A}\_x(\mathit{B}\_y\mathbf{\hat{k}} - \mathit{B}\_z\mathbf{\hat{j}})
\end{equation}

applying this to \\(\mathit{y}\\) and \\(\mathit{z}\\) components gives:

\\[

\begin{aligned}
\mathit{A}\_y\mathbf{\hat{j}}\times\mathbf{B} &= \mathit{A}\_y(\mathit{B}\_z\mathbf{\hat{i}} - \mathit{B}\_z\mathbf{\hat{k}}) \\\\
\mathit{A}\_z\mathbf{\hat{k}}\times\mathbf{B} &= \mathit{A}\_z(\mathit{B}\_x\mathbf{\hat{j}} - \mathit{B}\_y\mathbf{\hat{i}})
\end{aligned}

\\]

a simple way to remember this is to write the base vectors and the components of
\\(\mathbf{A}\\) and \\(\mathbf{B}\\) as three rows of a determinant:

\\[

\begin{aligned}
\mathbf{A}\times\mathbf{B} &=
\begin{vmatrix}
\mathbf{\hat{i}} & \mathbf{\hat{j}} & \mathbf{\hat{k}} \\\\
\mathit{A}\_x     & \mathit{A}\_y     & \mathit{A}\_z     \\\\
\mathit{B}\_x     & \mathit{B}\_y     & \mathit{B}\_z
\end{vmatrix} \\\\
&= \mathbf{\hat{i}}(\mathit{A}\_y\mathit{B}\_z - \mathit{A}\_z\mathit{B}\_y) - \mathbf{\hat{j}}(\mathit{A}\_x\mathit{B}\_z - \mathit{A}\_z\mathit{B}\_x) + \mathbf{\hat{k}}(\mathit{A}\_x\mathit{B}\_y - \mathit{A}\_y\mathit{B}\_x)
\end{aligned}

\\]

plugging in \\(\mathbf{A} = \mathbf{\hat{i}} + 3\mathbf{\hat{j}} - \mathbf{\hat{k}}\\) and \\(\mathbf{B} = 4\mathbf{\hat{i}} + \mathbf{\hat{j}} + 3\mathbf{\hat{k}}\\):

\\[

\begin{aligned}
\mathbf{A}\times\mathbf{B} &=
\begin{vmatrix}
\mathbf{\hat{i}} & \mathbf{\hat{j}} & \mathbf{\hat{k}} \\\\
1                & 3                & -1               \\\\
4                & 1                & 3
\end{vmatrix} \\\\
&= 10\mathbf{\hat{i}} - 7\mathbf{\hat{j}} - 11\mathbf{\hat{k}}
\end{aligned}

\\]


### displacement and the position vector {#displacement-and-the-position-vector}

vectors are perfect for describing **kinematical laws**, or the laws governing the
geometric properties of motion.

to locate the position of a point in space, we must first set up a coordinate
system. for convenience we select the three-dimensional cartesian system with
axes \\(\mathit{x}\\), \\(\mathit{y}\\), and \\(\mathit{z}\\).

in order to measure position, we have to mark these axes off in a convenient
unit of length, meters for instance. then you give its values of the three
coordinates, \\(x\_1, y\_1, z\_1\\). if we move this to a new position, \\(x\_2, y\_2,
z\_2\\), then the **displacement** defines a vector \\(\mathbf{S}\\) with coordinates
\\(\mathit{S}\_x = x\_2 - x\_1, \mathit{S}\_y = y\_2 - y\_1, \mathit{S}\_z = z\_2 - z\_1\\).

{{< figure src="/assets/displacement-vector.png" >}}

this vector defines displacement of a point of interest, it contains no
information about the initial and final positions seperately, only about the
relative positions of each. Thus, \\(\mathit{S}\_z = z\_2 - z\_1\\) depends on the
_difference_ between the final and initial values, but it doesn't specify the
values seperately. additionally, the values of the coordinates depend on the
coordinate system, but the vector itself does not.

a convention used is that a magnitude of a vector has dimensions so the unit
vectors are dimensionless. for example, a displacement of 8 meters in the \\(x\\)
direction is \\(\mathbf{S} = (8m, 0, 0)\\). \\(\lvert\mathbf{S}\rvert = 8m\\), and
\\(\mathbf{\hat{S}} = \frac{\mathbf{S}}{\lvert\mathbf{S}\rvert} = \mathbf{\hat{i}}\\).
