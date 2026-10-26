# Special Relativity

## Postulates of Special Relativity

> Time is that which is measured by a clock. An ideal clock is a proxy for time.

1. The laws of physics are the same in all inertial reference frames.
2. The speed of light is independant of the speed of the source/ the speed of light is invariant

## Time Dilation

Consider a light clock that is made up of a source and two mirrors. The light leaves the bulb, is reflected by a mirror and returns back to the first mirror, each round trip interval 'tick' is $\Delta t$. It travels some $\Delta x$ vertically up and down between the two mirrors.

If the clock begins moving suddenly at a velocity of $v$ which is very close to the speed of light. If the distance between the two mirrors stays the same then the time it takes the light to move to the next mirror is increased by pythagoras' theorem

```math
\left(\frac{c \Delta t}{2} \right)^{2} = \left(\frac{v \Delta t}{2} \right)^{2} + \Delta y^{2}
```

> We will use $O'$ to signify the frame of the clock and $O$ to show our perspective reference frame.

In the clock's perspective, the length stays the same which means that the time it experiences is the same.

```math
\text{In the reference of the clock}: \newline
\Delta y = \Delta y' = \frac{c \Delta t}{2}
```

```math
c^{2}\Delta t^{2} = v^{2}\Delta t^{2} + c^{2}\Delta t'^{2}
\newline
\Delta t^{2} = \frac{v^{2}}{c^{2}}t^{2} + \Delta t'^{2}
\newline
\Delta t^{2} \left(1 - \frac{v^{2}}{c^{2}}\right) = \Delta t'^{2}
```

```math
\Delta t = \frac{\Delta t'}{\sqrt{1 - \frac{v^{2}}{c^{2}}}}
```

Where $\gamma$ takes values: $1 \leq \gamma < \infty$:

```math
\gamma = \frac{1}{\sqrt{1 - \frac{v^{2}}{c^{2}}}}
```

```math
\Delta t = \gamma \Delta t'
```

## Length Contraction

Consider the same beam of light but instead of traveling vertically (or perpendicular to the direction of travel), it moves horizontally or parallel to the direction.

It moves to the right in the time $\Delta t'_{1}$ then bounces back and travels to the source in a time $\Delta t'_{2}$. In the frame of the clock, $O'$, they should be the same.

```math
d'_{1} = \Delta x' = c \Delta t'_{1}
```

And:

```math
d'_{2} = \Delta x' = c \Delta t'_{2}
```

As well as $d'_{1} = d'_{2} = d = \Delta x$, but in the frame of $O$, the distance that the light has to travel is two different lengths.

From reference frame $O$

```math
d_{1} = \Delta x + v \Delta t_{1}
```

But also:

```math
d_{1} = c \Delta t_{1}
```

So

```math
c \Delta t_{1} = \Delta x + v \Delta t_{1}
```

```math
\Delta t_{1} = \frac{\Delta x}{c-v}
```

On the way back the distance is now this because the clock is moving a non-negligible distance while the light is travelling

```math
d_{2} = \Delta x - v \Delta t_{2}
```

Also

```math
d_{2} = c \Delta t_{2}
```

So

```math
c \Delta t_{2} = \Delta x - v \Delta t_{2}
```

```math
\Delta t_{2} = \frac{\Delta x}{c+v}
```

Total time must be

```math
\Delta t = \Delta t_{1} + \Delta t_{2} = \frac{\Delta x}{c-v} + \frac{\Delta x}{c+v} = \frac{2c \Delta x}{c^{2}-v^{2}}
```

```math
\Delta t = \frac{2 \Delta x}{c(1-\frac{v^{2}}{c^{2}})}
```

And we know that

```math
\Delta t = \frac{\Delta t'}{\sqrt{1-\frac{v^{2}}{c^{2}}}}
```

For reference frame $O'$

```math
\Delta t' = \Delta t'_{1} + \Delta t'_{2} = \frac{\Delta x'}{c} + \frac{\Delta x'}{c} = \frac{2\Delta x'}{c}
```

Substitution gets us

```math
\Delta t = \frac{\Delta t'}{\sqrt{1-\frac{v^{2}}{c^{2}}}} = \frac{2\Delta x'}{c\sqrt{1-\frac{v^{2}}{c^{2}}}}
```

So

```math
\frac{2\Delta x}{c(1- \frac{v^{2}}{c^{2}})} = \frac{2\Delta x'}{c\sqrt{1-\frac{v^{2}}{c^{2}}}}
```

```math
\Delta x = \sqrt{1-\frac{v^{2}}{c^{2}}} \Delta x'
```

```math
\Delta x = \frac{\Delta x'}{\gamma}
```

This implies that objects moving close to or at the speed of light will shorten in the direction they travel from the perspective of someone outside the clock

Proper time $\tau$ is a property given to every object

## Lorentz Transformations

A reference frame $O$ has coordinates $x,y,z,t$ whilst a different reference frame $O'$ has coordinates $x',y',z',t'$ each measured relative to the origin reference.

A single point in space and time is an event, it can be described by either systems

Often we want to find how the primed variables relate to the non prime ones as functions. Events happen regardless of the coordinate system.

Take for example lining up the x axis of $O$ and the x' axis of $O'$ with the direction of the relative velocity $v$ between the reference frames

```math
\Delta y' = \Delta y, \, \Delta z' = \Delta z
```

Consider a train moving with velocity $v$ relative to the platform. Where the platform has $O$ and the train has $O'$, and $t= t' = 0$

Let A denote the end of the train that the light pulse is beeing fired from and B as the front of the train by which is the receiver

In $O'$ the interval in the $x'$ direction is $\Delta x'$ and the time interval is $\Delta t' = \frac{\Delta x'}{c}$

$\Delta x'$ is also the proper length $L$. As the light moves from the back to the front, the platform moves an amount $v\Delta t'$ that is Lorentz contracted

```math
\Delta x' + v\Delta t' = \frac{\Delta x}{\gamma} \implies \Delta x = \gamma (\Delta x' + v \Delta t')
```

This argument could reverse the primes in the perspective of $O$

```math
\Delta x' = \gamma (\Delta x + v \Delta t)
```

## Simultaneity/ Synchronisation

Consider a light source equally spaced between clocks A and B in one rest frame, when the clocks detect a pulse, they reset. Now consider that the clocks are on opposite ends of the moving train with A at the back. The time it takes for the light to travel to A is $\Delta t_{A}$

```math
c\Delta A + v\Delta t_{A} = \frac{L}{2\gamma} \quad \rightarrow \quad \Delta t_{A} = \frac{L}{2\gamma (c+v)}
```

Similarly, the time it takes the light to travel from the source to clock B at the front is $\Delta t_{B}$ and is given by

```math
c\Delta B + v\Delta t_{B} = \frac{L}{2\gamma} \quad \rightarrow \quad \Delta t_{B} = \frac{L}{2\gamma (c-v)}
```

In the rest frame, the time difference should be 0 but in the other rest frame, it will be non zero

```math
\Delta t_{B} - \Delta t_{A} = \frac{L}{2\gamma (c-v)} - \frac{L}{2\gamma (c+v)} = \gamma \frac{vL}{c^{2}}
```

This shows that simultaneity is a property of the reference frame, and not an intrinsic property of two clocks.
