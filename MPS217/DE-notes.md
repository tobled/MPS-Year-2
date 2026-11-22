# Differential Equations

## Classification

### Independant or Dependent Variables

```math
\frac{dy}{dx}=x^{2}
```

Here, $y$ depends on $x$, so $x$ is the independent and $y$ is the dependant variable

### Ordinary or Partial

```math
\frac{dy}{dx}=x^{2}
```

This is an ordinary differential equation because there is only one independent variable

```math
\frac{\partial y}{\partial x}=\frac{1}{c^{2}} \frac{\partial^{2}y}{\partial t^{2}}
```

This is a partial differential equation becauses there is more than one independent variables

### Linear or Non-Linear

```math
\frac{dy}{dx}=x^{2}
```

An equation is linear if the highest power of the dependent variable or any of its derivatives is one

```math
\frac{dy}{dx}=y^{2}
```

A non-linear equation contains higher powers:

```math
\frac{dy}{dx} = \, \text{sin} \, y
```

This is also non linear because of the taylor expansion that has higher powers of increasing $y$

### Order of an Equation

```math
\frac{dy}{dx}=y^{2}
```

This is a first order because it contains the first derivative of y, however:

```math
\frac{d^{2}y}{dx^{2}}+ \frac{dy}{dx} +y = 0
```

Is second order

### Homogenous or Inhomogeneous

```math
\frac{d^{2}y}{dx^{2}}+ \frac{dy}{dx} +y = 0
```

This is homogeneous because all terms contain the dependant variable $y$

```math
\frac{dy}{dx}=x^{2}
```

This is inhomogeneous because RHS does not have the dependent variable

## First Order DEs

Use the separation of variables method to solve these

```math
\frac{d^{2}y}{dx^{2}}=x^{2}
```

```math
\frac{dy}{dx}=\frac{x^{3}}{3}+A
```

```math
y = \int \left(\frac{x^{3}}{3}+A\right)dx = \frac{x^{4}}{12}+Ax+B
```

> Remember constant if indefinite

## Second Order DEs: Homogeneous

### Superposition Principle

If $f(x)$ and $g(x)$ are solutions to the equation then so is the linear combination

```math
y=Af(x)+Bg(x)
```

> A, B are arbitrary constants

We can say that the general solution to an equation is an arbitrary linear combination of two possible solutions

For first order DEs, there is mainly just one solution so the superposition principle is less useful here compared to second order DEs

## Constant Coefficients

For an equation like this:

```math
a\frac{d^{2}x}{dt^{2}} + b\frac{dx}{dt} + cx = 0
```

It has solutions of the form $x = e^{mt}$:

```math
\frac{dx}{dt} = me^{mt} = mx \qquad \frac{d^{2}x}{dt^{2}} = m^{2}e^{mt} = m^{2}x
```

```math
am^{2}+bm+c=0
```

Solve for $m$, then write generel solution as:

```math
x=Ae^{m_{1}t}+Be^{m_{2}t}
```

This forms the idea for the auxiliary equation which could imply that the roots of $m$ are:

1. Real and distinct
2. Real and identical
3. Complex and in a conjugate pair

> use discriminant to determine which option best describes $m$

### General Solutions 1

#### Real and Distinct

```math
x(t) = Ae^{m_{1}t} + Be^{m_{2}t}
```

#### Real and Identical

```math
x(t) = (A + Bx)e^{mt} \qquad m=m_{1}=m_{2}
```

#### Complex Roots

```math
x(t) = e^{\alpha t}(A' \, \text{cos} \,(\beta t) + B' \, \text{sin} \,(\beta t)) \qquad m = \alpha \pm i\beta
```

## Boundary Conditions

Uses boundaries to find the values of the arbitrary constants, they are made explicit in the question with bounds like:

```math
x(0) = k \quad x'(0) = v_{0}
```

### Complementary Functions and Particular Integrals

> $D$ is the differential operator

Complementary functions refer to the LHS with the second order DE whilst the Particular integral refers to the RHS that it equals. It is the inhomogeneous term.

```math
x = x_{c}+x_{p}
```

For Example:

```math
\frac{d^{2}x}{dt^{2}}+4x =  \, \text{sin} \,t
```

Find Auxiliary

```math
m^{2}+4=0
```

We find that $m=\pm 2i$, so the complementary function is

```math
x_{c}(t) = A \, \text{sin} \,2t + B \, \text{cos} \,2t
```

Particular integral takes the form:

```math
x_{p} = a \, \text{cos} \, t + b \, \text{sin} \, t
```

Differentiate:

```math
\frac{dx_{p}}{dt} = -a  \, \text{sin} \, t + b  \, \text{cos} \, t \qquad \frac{d^{2}x}{dt^{2}} = -a \, \text{cos} \, t - b \, \text{sin} \, t
```

Substitute into the DE:

```math
(-a  \, \text{cos} \,t - b \, \text{sin} \,t)+4(a \, \text{cos} \,t + b \, \text{sin} \, t) =  \text{sin} \,t
```

Compare coefficients:

```math
-a + 4a = 0 \qquad -b + 4b = 1
```

```math
x_{p}=\frac{1}{3} \, \text{sin} \, t
```

The full solution is now

```math
x(t) = x_{c}(t) + x_{p}(t) = A \,\text{sin}\, 2t + B \,\text{cos}\, 2t + \frac{1}{3} \, \text{sin} \, t
```

#### Complex case

```math
x_{p}(t) = ae^{2it}
```

then there will be only one arbitrary constant to be found

## Partial DEs

### Examples

#### The Wave Equation

```math
\nabla^{2}u = \frac{1}{c^{2}} \frac{\partial^{2u}}{\partial t^{2}}
```

$u$ is the displacement of the wave. $\nabla^{2}$ is the Laplacian operator which is $\frac{\partial^{2}u}{dx^{2}}$ in one dimension and $c$ is the speed of the wave

#### The Laplace Equation

```math
\nabla^{2}u = 0
```

Applies to many systems i.e., $u$ is a potential in electrostatics, gravitation, hydrodynamics

#### The Diffusion Equation

```math
\nabla^{2}u = \frac{1}{h^{2}}\frac{\partial u}{\partial t}
```

Describes the diffusion of gases, heat. $u$ is the density or temperature. $h^{2}$ is the diffusion constant

#### The Schrödinger Equation

```math
-\frac{\hbar^{2}}{2m} \nabla^{2} \psi + V\psi = i\hbar \frac{\partial \psi}{\partial t}
```

Where $\psi$ is the wavefunction, $V(r)$ is the potential, $m$ is the particle mass and $\hbar$ is Planck's constant divided by $2\pi$

## Wave Equation in 1D

Consider the one dimensional wave equation:

```math
\frac{\partial^{2}u}{\partial x^{2}} = \frac{1}{c^{2}} \frac{\partial^{2}u}{dt^{2}}
```

Where $u(x,t)$ is the displacement of the string. Speed of the wave $c = \sqrt{T/\mu}$. Consider the boundaries $x=0$ and $x=L$ which makes $u(0,t) = 0 = u(L, t)$

### Separating Variables

The boundary conditions must be satisfied at special values of $x$ but for all values of $t$. Let our solution take the form:

```math
u(x,t) = X(x)T(t)
```

Where $X$ is a function of only $x$ and $T$ is a function of only $t$. Sub in this solution and separate:

```math
\frac{1}{X(x)} \frac{d^{2}X(x)}{dx^{2}} = \frac{1}{c^{2}} \frac{1}{T(t)}\frac{d^{2}T(t)}{dt^{2}}
```

Because X and T are made up of one same variable, you can drop the partials:

```math
\frac{1}{X} \frac{d^{2}X}{dx^{2}} = \frac{1}{c^{2}T}\frac{d^{2}T}{dt^{2}}
```

The only way that this equation is satisfied is if LHS and RHS equal a constant, $N$:

```math
\frac{d^{2}X}{dx^{2}} = NX \qquad \frac{d^{2}T}{dt^{2}} = Nc^{2}T
```

> If $N<0$ then it is a harmonic oscillator, if $N>0$ then the solutions are exponentially growing or decaying, these signs can be found when thinking about the underlying physics or more mathematically by satisfying boundary conditions

### Satisfy the Boundary Conditions

From our own bouyndary conditions, we see that there are two 0 points which mean that out solution is harmonically oscillating, therefore, $N<0$. Exponential functions cannot have two 0 points.

Rule out $N=0$ solution as it would take form of $X(x) = Ax + B$ which would need $A = 0 = B$ which is a trivial solution for all $x$

If $N>0$ like $N = k^{2}$ with k real, the general solution would be $X(x) = Ae^{-kx}+Be^{-kx}$ which can also only be satisfied if $A = 0 = B$ giving $X(x)=0$ for all $x$

Therefore N must be negative, let $N = -k^{2}$:

```math
\frac{d^{2}X}{dx^{2}} = -k^{2}X
```

With general solution:

```math
X(x) = A\text{cos}kx + B\text{sin}kx
```

Use the boundary conditions $X(0) = A \rightarrow A = 0$ and $X(L) = B \text{sin}(kL)$.

$B \neq 0$ as that would be the trivial solution so $\text{sin}(kL) = 0$ giving:

```math
k = k_{n} = \frac{n\pi}{L}
```

Where $n$ is any integer but 0

```math
X_{n}(x) = B_{n} \text{sin} \left(\frac{n\pi x}{L}\right) \qquad \text{for} \; n = 1,2,3,...
```

With values of $k$ and now $N$

```math
\frac{d^{2}T}{dt^{2}} = Nc^{2}T = -k^{2}_{n}c^{2}T = -\frac{n^{2}\pi^{2}c^{2}}{L^{2}}T = -omega_{n}^{2}T
```

This has the form of a harmonic oscillator as well so:

```math
T_{n}(t) = C_{n}\text{sin}(\omega_{n}t) + D_{n}\text{cos}(\omega_{n}t) \qquad \text{or} \qquad C_{n}\text{cos}(\omega_{n}t + \phi_{n})
```

More constraints are necessary to solve further, that being, initial conditions

```math
u_{n}(x,t) = X_{n}(x)T_{n}(t) = B_{n} \text{sin} (k_{x}x) \text{cos}(\omega_{n}t + \phi_{n}) = B_{n} \text{sin} \left(\frac{n\pi x}{L}\right) \text{cos}\left(\frac{n\pi ct}{L} + \phi_{n}\right)
```

These solutions desscribe the fundamental and harmonics of the standing waves on a string.

### General Solution

Use the superposition principle to form the most general solution that satisfies the boundary conditions

> Superposition principle applies to any linear and homogeneous differential equation - the dependent variable ($u$ in the wave equation) and its derivatives only appear as the first power.
>
> It states that if $u_{1}$ and $u_{2}$ are solutions to the equation, then $u = c_{1}u_{1} + c_{2}u_{2}$ with both $c$ as arbitrary constants, is also a solution.

Thus, any linear combiation of our sstanding wave solutions will also be a solution to the wave equation, satisfying the same boundary conditions:

```math
u(x,t) = \sum^{\infty}_{n=1} B_{n} \text{sin} \left(\frac{n\pi x}{L}\right) \text{cos}\left(\frac{n\pi ct}{L} + \phi_{n}\right)
```

> This form is no longer separable in the form $u(x,t) = X(x)T(t)$

### Satisfy the Initial Conditions

To find the values of the arbitrary constants we need to know what the function is doing at a point in time i.e., $t=0$.

Take for axample, the string being held initially in a triangular shape, displaced by a distance $d$ at $L/2$ before being released:

$$
u(x,0) =
\begin{cases}
  2dx/L & 0 \leq x \leq L/2 \\
  2dx/(1-x/L) & L/2 \leq x \leq L
\end{cases}
$$

Calculating the velocity:

```math
\frac{\partial u}{\partial t} = \sum^{\infty}_{n=1} -B_{n} \frac{n\pi c}{L} \text{sin} \left(\frac{n\pi x}{L}\right) \text{sin}\left(\frac{n\pi ct}{L} + \phi_{n}\right)
```

For velocity to be zero everywhere at $t=0$, $\phi_{n} = 0$

```math
u(x,t) = \sum^{\infty}_{n=1} B_{n} \text{sin} \left(\frac{n\pi x}{L}\right) \text{cos}\left(\frac{n\pi ct}{L}\right)
```

```math
u(x,0) = \sum^{\infty}_{n=1} B_{n} \text{sin} \left(\frac{n\pi x}{L}\right)
```

This is close to a Fourier series, more specifically, a half-range sine Fourier series, hence, we can use the same expansions to calculate our $B_{n}$:

```math
B_{n} = \frac{2}{L} \int_{0}^{L} f(x) \text{sin} \left(\frac{n\pi x}{L}\right) dx
```

This calculates as:

$$
B_{n} =
\begin{cases}
  -\frac{8d}{\pi^{2}}\frac{1}{n^{2}}(-1)^{(n+1)/2} & \text{for odd }n \\
  0 & \text{for even }n
\end{cases}
$$

### Summary

```math
\frac{1}{X(x)} \frac{d^{2}X(x)}{dx^{2}} = \frac{1}{c^{2}} \frac{1}{T(t)}\frac{d^{2}T(t)}{dt^{2}}
```

1. Look for a seperable solution $u(x,t) = X(x)T(t)$ and write the wave equation as above
2. Consider boundary conditions, decide the sign of N. If negative, $N = -k^{2}$. Solve for X(x) finding the allowed values of $k$ and so, $k_{n}$
3. Use $k_{n}$ to find $T(t)$
4. Apply superposition principle to express the general solution as a linear combination of the separable solutions which gives the most general solution for our BC
5. Use a Fourier expansion to determine the arbitrary constants in the general solution from the initial conditions

> This is not the only method to solving PDE's, in fact D'Alembert uses a different approach to find the solution using completely arbitrary functions
