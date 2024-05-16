---
layout: page
permalink: research_intro
---


An initial encounter with polynomial interpolation might involve Lagrange interpolating polynomials. Given $k$ pairs of real numbers $(x_i,y_i)$ with $x_i$ distinct and $y_i$ arbitrary, there is always a unique polynomial $f\in \mathbb{R}[x]$ such that $f(x_i)=y_i$ for each $i=1,2,\dots,k$ with $\deg{f}\le k-1$. A student with a background in calculus can easily verify that the polynomial

$$ f(x)=\sum_{i=1}^{k}y_i\prod_{j=1,j\ne i}^{k}\frac{x-x_j}{x_i-x_j}$$ 

does precisely that.

The complexity of the interpolation problem increases significantly when the problem is posed in higher dimensions. In $\mathbb{R}^2$, the problem begins with a collection of $k$ distinct points $(x_i,y_i)\in \mathbb{R}^2$ and arbitrary values $z_i$ and we ask whether there is a polynomial $g(x,y)$ such that $g(x_i,y_i)=z_i$ for each $i=1,2,\dots,k$. We may recontextualize the problem using linear algebra to give a new perspective.

As an example, consider three points $(x_1,y_1),(x_2,y_2)$, and $(x_3,y_3)$ in $\mathbb{R}^2$. We may ask whether there is a linear polynomial $h(x,y)=ax+by+c$ such that $h(x_i,y_i)=0$. This information may be described in the matrix 

$$\begin{pmatrix}x_1 & y_1 & 1  \\ x_2 & y_2 & 1  \\ x_3 & y_3 & 1 \end{pmatrix} \begin{pmatrix} a \\ b \\ c\end{pmatrix}=\begin{pmatrix} 0 \\ 0 \\ 0 \end{pmatrix}.$$

While the invertible matrix theorem gives conditions on whether the above system is consistent, observe that if such a solution $(a,b,c)$ exists, it corresponds to a line with the equation $ax+by+c=0$. For the $3$ points to satisfy this one equation, that would imply that the $3$ points would need to be collinear. On the other hand, if the $3$ points were not collinear, then no such $(a,b,c)$ exists that satisfies the system. This is a first example of how the position of the initial points matters greatly, unlike in the one-dimensional case where the distinct points $x_i$ could be chosen arbitrarily.


The interpolation problem is similar to finding polynomials vanishing at points, and that is the starting point of Algebraic Geometry. One quickly encounters difficult interpolation problems, for example, given a collection of points $\{p_i=(x_i,y_i)\}\in \mathbb{R}^2$ with a multiplicity $m_i$ assigned at each point $p_i$, it is an open question to determine the minimum value $d$ for which there is a non-zero polynomial of degree $d$ vanishing to order at least $m_i$ at each $p_i$. If the points exhibit some symmetry or structure, this impacts what polynomials vanish at the points, as in the case of collinear points. That is, a *general* collection of points and a *special* collection of points will exhibit different spaces of vanishing polynomials. My research interest includes interpolation problem for special collections of points that are symmetric under some group action. 