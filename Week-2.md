# Week 2

*October 24, 2018*

## Table of Indefinite Integral

Some common integrals

$\int \frac{1}{x^2+1}dx = arctan x + C$ 

$\int \frac{1}{\sqrt{1-x^2}}dx = arcsin x + C$

## Substitution Rule 

**Theorem**: The Substitution Rule

> $\int f(g(x))g'(x)dx = \int f(u) du$, where $u = g(x)$.

**Examples**

> Evaluate $\int x^{3} sin(x^4+9)dx$  

> Evaluate $\int \sqrt[3]{4x+1} dx$ 

> Evaluate $\int tan x dx $

​	$-ln\:cos x + C$

> Evaluate $\int sec^4{3\theta}d\theta$ 

 	$\frac{1}{3}(tan3\theta+ \frac{tan^{3}3\theta}{3})+C$ 

## Integration by Parts

Let $u$ and $v$ be differentiable functions on the same interval. Then 

$$\frac{d(uv)}{dx} = u\frac{dv}{dx} + v\frac{du}{dx}$$     

Integrate both sides with respect to $dx$ and we obtain

$\int udv = uv-\int vdu$

**Examples**

> Evaluate $\int x cosx dx$ 

​	Let $u = x$ and $du = cos x dx$. Then $du = dx$ and $u = sinx + C_1$. 

​	$\int xcosx = x(sinx+C_1) - \int(sinx+C_1)dx$ 

​			$ = xsinx +C_1x + cosx - C_1x+C_2$

​			$ = xsinx + cosx + C$ 

> Evaluate $\int xe^{x} dx$  

> Evaluate $\int lnx dx$ 

> Evaluate $\int cos(lnx) dx$ 

​	$\frac{1}{2}(xsinlnx+xcoslnx)+C$  

> Evaluate $\int e^{ax} cos bx dx$, where $a, b \in \mathbb{R}$ such that $a^2 + b^2 > 0$  

​	$\frac{1}{a^2+b^2}(be^{ax}sinbx+ae^{ax}cosbx)+C$

> Evaluate $\int sin \sqrt{x} dx$ 

## Trigonometric Integrals

An important trigonometric identity is

$cos2x = cos^2x - sin^2 x = 2cos^2x-1 = 1-2sin^2x$ 

**Theorem** The Binomial Theorem

> $(x+y)^k =\:...$ 

**Strategies** for evaluating $\int sin^m xcos^nxdx$

1. If $n$ is odd, save one cosine factor and use $cos^2x = 1-sin^2x$ to express the remaining factors in terms of $sinx$, then substitute $u = sinx$ 

   ​	$sin^mxcos^{2k+1}x = sin^mx(1-sin^2x)^kcosxdx$

2. If m is odd, save one sine factor and use $sin^2x = 1-cos^2x$ to express the remaining factors in terms of $cosx$, then substitute $u = cosx$ 

   ​	$sin^{2k+1}xcos^nx = (1-cos^2x)^kcos^nxsinx$

3. If m and n are even, use the half-angle identities $sin^2x = \frac{1}{2}(1-cos2x)$, $cos^2x = \frac{1}{2}(1+cos2x)$, then expand and solve.

   ​	$sin^{2m}cos^{2n}x = \frac{1}{4}(1-cos2x)^{m}(1+cos2x)^{n}$ 

**Examples** 

> Evaluate $\int sin^2xcos^2xdx$ 

**Strategies** for evaluating $\int tan^mxsec^nxdx$

1. If $n$ is even, save a factor $sec^2x$ and use $sec^2x = 1+tan^2x$ to express the remaining factors in terms of  $tan x$ , then substitute $u = tanx$.

   ​	$tan^mxsec^{2k}x = tan^mx(1+tan^2x)^{k-1}sec^2x$  

2. If $m$ is odd, save a factor of $secxtanx$ and use $tan^2x = sec^2x - 1$ to express the remaining factors in terms of $sec x​$.

3. If $m$ is even and $n$ is odd, use $tan^2x = sec^2x-1$ to express the factor in terms of $sec x$.

   ​	$tan^{2k}sec^{2l+1}xdx = (sec^2x-1)^ksec^{2l+1}$ 

   and use the binomial theorem to expand the term. Note that the powers of all the terms are odd.

   Next, we consider $\int sec^qxdx$, where $q$ is odd.

   Take u = $sec^{q-2}xdx$ and $dv = sec^2{x}dx$. 

   Then $\int sec^qxdx = sec^{q-2}xtanx-(q-2)\int sec^{q-2}xtan^2xdx$ 

   ​				$ = sec^{q-2}xtanx- (q-2)\int sec^qxdx + (q-2)\int sec^{q-2}xdx$ 

   ​	$(q-1)\int sec^{q}xdx = sec^{q-2}xtanx + (q-2)\int sec^{q-2}xdx​$ 

   Finally, we have $\int sec^qxdx = \frac{sec^{q-2}xtanx}{q-1}+\frac{q-2}{q-1}\int sec^{q-2}xdx$.

   We continue this process until the power of secant is 1.

   This is called a *reduction formula* as the problem is reduced to lower indices of $sec^qx$ and the parity stays the same.  

**Examples**

> Evaluate $\int sec^5xtan^3xdx$ 

> Evaluate $\int sec^3xdx$ 