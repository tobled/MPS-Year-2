# Fourier Techniques and Optics

## Fourier Series

Fourier series are applied to situations where we have a continuously repeating, periodic function of time or distance

Any periodic function can be described by a Fourier series consisting of an infinite number of sine and/or cosine terms of frequencies equal to the fundamental frequency of the original function plus its harmonics

If $f(t)$ is periodic then use a Fourier series and if $f(t)$ is non-periodic then use a Fourier transform

The frequency components will be $nf_{0}$ where $n=1,2,3...\infty$, it tells us how much of each frequency is present

Consider a sine wave, it is easy to write in the form of a differential equation i.e., $m \frac{d^{2}x}{dt^2} + \gamma \frac{dx}{dt} + kx = Asin(\omega t)$. For a square wave, this is much more difficult and requires a Fourier series representation i.e., $m \frac{d^{2}x}{dt^2} + \gamma \frac{dx}{dt} + kx = A'\sum^{\infty}_{n=1(odd)} \frac{1}{n}sin(n\omega t)$

If $f(t)$ is a periodic function of period T then the Fourier series for $f(t)$ is:

```math
f(t) = \frac{1}{2}a_{0} + \sum^{\infty}_{n=1} \left(a_{n}cos\frac{2n\pi t}{T} + b_{n}sin\frac{2n\pi t}{T}\right) \quad n=1,2,3...\infty
```

Where:

```math
a_{0} = \frac{2}{T} \int_{0}^{T} f(t)dt \qquad a_{n} = \frac{2}{T}\int_{0}^{T}f(t)cos\frac{2n\pi t}{T}dt \qquad b_{n} = \frac{2}{T}\int_{0}^{T}f(t)sin\frac{2n\pi t}{T}dt
```

> These can be written similarly for $f(x)$ of period $L$, any limit evaluated for an integral over one period is valid.

If $T=2\pi$ then:

```math
f(t) = \frac{1}{2}a_{0} + \sum^{\infty}_{n=1} \left(a_{n}cos \, nt  + b_{n}sin \, nt \right) \quad n=1,2,3...\infty
```

Where:

```math
a_{0} = \frac{1}{\pi} \int_{0}^{2\pi} f(t)dt \qquad a_{n} = \frac{1}{\pi}\int_{0}^{2\pi}f(t)cos \, nt \, dt \qquad b_{n} = \frac{1}{\pi}\int_{0}^{2\pi}f(t)sin \, nt \, dt
```

$\frac{a_{0}}{2}$ is sthe average of $f(t)$ over one period.

> Equations are given in the exam

### Series Symmetry

> Symmetry and Parity refer to the same idea

Many functions have even or odd symmetry (some have neither). All terms in a Fourier series must have same symmetry as the original function. For example, if $f(x)$ is an even function then there will only be terms with $cos(nx). Alternatively, if $f(x)$ is odd then only $sin(nx)$ will be present

> A constant has even symmetry, this is why we only have $a_{0}$

The product of $f(x)$ and its trig function will likely result in an even function which can be used to simplify the integral they are under:

```math
\frac{2}{L}\int^{\frac{L}{2}}_{\frac{-L}{2}} (even \, function)dx = 2 \times \frac{2}{L}\int^{\frac{L}{2}}_{0} (even \, function)dx
```

> Do not confuse the lower bound of the summation to indicate the symmetry of the function

### Half Range Series

Some functions may have a limited range over say, $0 \rightarrow L$, we can use the Fourier series by assuming that this range is repeating with periodicity $L$

> If a repeating function is neither odd or even then assume that there will be both cosine and sine terms

We can make it easier by forcing the periodicy to be $2L$ allowing forced symmetry

### Frequency Spectra

The values of $a_{n}$ and $b_{n}$ tell us which frequency components are present in the function and their amplitudes.

A square wave has frequency components $f_{0}, \, 2f_{0} \, 3f_{0} \, 4f_{0} \, 5f_{0}...$ with relative amplitudes 1:0:1/3:0:1/5...

This can be plotted on a graph of $F(f)$ against $f$

## Fourier Transforms

As $T \rightarrow \infty$ the fundamental frequency $1/T \rightarrow 0$ and the harmonics get closer together, eventually it will be replaced with a continuous distribution of frequencies with the discrete summations replaced with an integral

```math
F(\omega) = \frac{1}{\sqrt{2\pi}} \int^{\infty}_{-\infty} f(t)e^{-i\omega t}dt \quad \mathrm{where} \quad  f(t) = \frac{1}{\sqrt{2\pi}} \int^{\infty}_{-\infty} F(\omega)e^{i\omega t}d\omega
```

```math
F(k) = \frac{1}{\sqrt{2\pi}} \int^{\infty}_{-\infty} f(x)e^{-ikx}dx \quad \mathrm{where} \quad f(x) = \frac{1}{\sqrt{2\pi}} \int^{\infty}_{-\infty} F(k)e^{ikx}dk
```

> $e^{i \theta} = cos \theta + i sin \theta$, $k = \frac{2\pi}{\lambda}$, $\omega = \frac{2\pi}{T}$, use $\omega$ rather than $f$ for posterity
>
> Equations are given in the exam

### Sinc Function

The Sinc function is defined as:

```math
sinc(x) = \frac{sin(x)}{x}
```

It spans between $\omega = \pm \infty$ but most of the intensity is between the first two zero points either side of $\omega = 0$. This means that the width of $F(\omega)$ is between the first two zeros.

The products of the widths of $f(t)$ and $F(\omega)$ are inversely proportional to each other and so, equal to a constant

### Transform Symmetry

```math
F(k) = \frac{1}{\sqrt{2\pi}} \int^{\infty}_{-\infty} f(x)e^{-ikx}dx = \frac{1}{\sqrt{2\pi}} \int^{\infty}_{-\infty} f(x)cos(kx)dx - \frac{i}{\sqrt{2\pi}} \int^{\infty}_{-\infty} f(x)sin(kx)dx
```

> This is also from $e^{i \theta} = cos \theta + i sin \theta$

If $f(x)$ is even then only the first integral is non-zero and $F(k)$ will be $\textbf{real}$, if $f(x)$ is odd then only the second integral is non-zero and $F(k)$ will be $\textbf{complex}$

If $f(x)$ is real and even then:

```math
F(k)=\frac{1}{\sqrt{2\pi}} \int^{\infty}_{-\infty} f(x) cos(kd) dx = \frac{2}{\sqrt{2\pi}} \int^{\infty}_{0} f(x) cos(kd) dx
```

### Dirac Delta Function

Consider a rectangular pulse of area 1 unit, we decrease the width until the height $\rightarrow \infty$ and width $\rightarrow 0$. This is the delta function $\delta (x)$. Total integral is still 1.

```math
\int_{-\infty}^{\infty} \delta (x) dx = 1 \quad \text{centred at} \, x=0
```

```math
\int_{-\infty}^{\infty} \delta (x-x_{0}) dx = 1 \quad \text{centred at} \, x=x_{0}
```

The product of the delta function with any function $f(x)$ is zero for all $x$ except where $x=x_{0}$

```math
\int_{-\infty}^{\infty} f(x) \delta (x-x_{0}) dx = f(x_{0})
```

## Convolution

Convolution is a mathematical process which takes 2 input functions $f(x)$ and $g(x)$and produces an output function.

> $f(x)$ is the responce of a measurement system and g(x) is the quantity being measured. The convolution gives what we actually measure, it tells us how the properties of our measurement system distort the quantity being measured.

A real detector would have a non-zero width but an ideal detector would have negligible thickness which distorts the measured profile

This is a problem because it could hide fine detail if present in the aperture

Often we see the measurement system has a Gaussian response and a single sharp feauture will give significant broadening, obscurring the output

### Convolution Definition

$f(x)$ is the system response function, $g(x)$ is the signal function

Introduce dummy variable $u$, enters as $f(u)$ and $g(x-u)$. Replot where $x$ is now a constant and the functions are offset by an amount $x$

For a given $x$, calculate the overlap between the two functions of $u$. Done by keeping $x$ constant and integrating the product of the two functions between $-\infty \rightarrow +\infty$ with respect to $u$

This gives a new function $c(x)$ which is the detected signal as a function of $x$. It is the convolution of the functions $f(x)$ and $g(x)$

```math
c(x) = f \ast g = \int^{\infty}_{-\infty} f(u)g(x-u)du
```

> Generally only performed using a computer

### Convolution with Delta Function

```math
c(x)=f \ast g = \int^{\infty}_{-\infty} \delta (u)g(x-u)du
```

```math
= \int^{\infty}_{-\infty} \delta (u)g(x)du = g(x)\int^{\infty}_{-\infty} \delta (u)du = g(x)
```

```math
g(x) = g(x) \ast \delta (x)
```

### Convolution Theorem and Deconvolution

If $C(k)$ is the Fourier transform of the convoluted function then:

```math
C(k) = \sqrt{2\pi} F(k)G(k)
```

To find $f(x)$

```math
F(k) =\frac{C(k)}{G(k)\sqrt{2\pi}} \qquad f(x) = \frac{1}{2\pi} \int^{\infty}_{-\infty} e^{ikx} \frac{C(k)}{G(k)}dk
```

The convolutiono of two Gaussian characterised by $a$ and $b$ is also a Gaussian characterissed by $\Delta$

The value of $\Delta$ is dominated by whichever is the smaller of $a$ or $b$, and is always ssmaller then either of them. The convolution of two Gaussians is always wider than either of the two startig functions
