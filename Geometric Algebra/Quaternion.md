# Quaternion

## **Definition**

$$
q = a + bi + cj + dk
$$

where

$$
i^2 = j^2 = k^2 = ijk =-1 \\
ij = k ~~~~ jk = i ~~~~ ki = j \\
ji = -k ~~~~ kj = -i ~~~~ ik = -j
$$

Also

$$
{\displaystyle \mathbf{q} =(r,\vec{v}) = r + \vec{v},~~ \mathbf{q} \in \mathbb{H} ,~~ r \in \mathbb{R} ,~~ \vec{v} \in \mathbb{R}^3,}
$$

$r$ is called its scalar part or real part, $\vec{v}$ is called its vector part or imaginary part.

## Addition

$q_1 = \alpha + \vec{a}$ and $q_2 = \beta + \vec{b}$, then

$$
q_1 + q_2 = (\alpha + \beta) + (\vec{a} + \vec{b})
$$

## Product (also called Hamilton product)

$$
q_1q_2 = (\alpha\beta - \vec{a} \cdot \vec{b}) + (\alpha\vec{b} + \beta\vec{a} + \vec{a} \times \vec{b})
$$

## **Conjugation**

$$
q^* = r - \vec{v} = a - bi - cj - dk
$$

$$
( q^* )^* = q  \\
(q_1q_2)^* = q_2^* q_1^* \\
qq* = a^2 + b^2 + c^2 + d^2
$$

## Norm

$$
\begin{Vmatrix}
q
\end{Vmatrix} 
= \sqrt{qq^*}
$$

and with real number $a$

  

$$
\begin{Vmatrix}
aq
\end{Vmatrix} 
= ||a||\sqrt{qq^*}
$$

and two quaternion $p$ and $q$

$$
\begin{Vmatrix}
pq
\end{Vmatrix} 
= \begin{Vmatrix}
p
\end{Vmatrix}
\begin{Vmatrix}
q
\end{Vmatrix}
$$

**reciprocal**

$$
q^{-1} = \frac{q^*}{||q||^2}
$$

Space geometry

A vector $\vec{V} = (x,y,z)$ can be seen as a quaternion which the scalar part is 0, i.g. $(0,x,y,z)$, so we can get a new vector $\vec{V}' = (0,x',y',z')$ :

$$
\vec{V}' = q\vec{V}q^*,~~\text{where }q\text{ is a unit quaternion}
$$

the norm of $\vec{V}'$ is equal $\vec{V}$

$$
||\vec{V}'||^2 = \vec{V}' {\vec{V}'}^* = q \vec{V} q^* ( q^* )^* \vec{V}^* q* = q \vec{V} q^* q \vec{V}^* q^* = q \vec{V} \vec{V}^* q^* = ||\vec{V}||^2 qq^* = ||V||^2 
$$

For any unit quaternion $q$, we can also rewrite as:

$$
q = \sin\frac{\theta}{2} + l\cos\frac{\theta}{2}
$$

where $\sin\frac{\theta}{2}$ is the scalar part of $q$, $l\cos\frac{\theta}{2}$ is the vector part of $q$.

So for a vector $\vec{V}$ and a unit quaternion $q$, the new vector $\vec{V}' = q\vec{V}q^*$ means:

the vector $\vec{V}$ rotate around axis $l$ with angle  $\theta$.
