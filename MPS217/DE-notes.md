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
