# Subatomic Particles

> **UNFINISHED, ADD PICTURES**

```math
\frac{mv_{0}^{2}}{2} = \frac{mv^{2}}{2} + \frac{Z_{1}Z_{2}e^{2}}{4 \pi \epsilon_{0} \delta}
```

Initial kinetic energy of a particle with velocity $v_{0}$ and impact parameter $b$ and scattered from the angle, $\theta$. Distance of closest approach $\delta$

```math
mbv_{0} = m \delta v 
```

```math
b = \frac{Z_{1}Z_{2}e^{2}}{4 \pi \epsilon_{0} mv_{0}^{2}} \cot \left( \frac{\theta}{2} \right)
```

## Cross Sectional Area

An example of an experiment which measures the cross section $\sigma$. The most commonly used unit for the cross section is the barn.

```math
\sigma = \frac{\text{Number of interactions/ time/ target particle}}{\text{Incident particle flux}}
```

> |Symbol|Measure|Unit|SI|
> |-|-|-|-|
> |$\sigma$|Cross Section|$1b$|$10^{-28}\mathrm{m^{2}}$|
> |$\phi$|Flux of Incident Beam|-|$\text{in particles} \cdot m^{-2}s^{-1}$|
> |$N_{target}$|No. of target particles|-|-|
> |$R$|Rate of observed scattering events|-|$s^{-1}$|

```math
R = \phi N_{target} \sigma
```

Cross section is the effective area taken out of the incoming beam of particles by each particle in the target. The cross section for scattering into an angle between $\theta$ and $\theta + d\theta$ is just the area of the ring. Using the integral to find the cross section for angle $\geq \theta$

```math
\sigma = \int_{0}^{b(\theta)} 2 \pi b \,db = \pi b^{2}(\theta)
```

## Alpha Particle Scattering

Take a setup that uses an alpha particle beam directed at a platinum foil.

> |Quantity|Unit|
> |-|-|
> |$E_{kin}$|$5\, \mathrm{MeV}$|
> |$d$|$1.2 \times 10^{-4} \text{cm}$|

We wish to find the fraction of particlse scattered by an angle $\theta \geq 90^{\circ}$ using $b$

```math
b = \frac{Z_{1}Z_{2}e^{2}}{4 \pi \epsilon_{0} mv_{0}^{2}} \cot \left( \frac{\theta}{2} \right)
```

If $mv_{0}^{2} = 2 E_{kin}$

```math
b = \frac{Z_{\alpha}Z_{Pt}e^{2}}{8 \pi \epsilon_{0} E_{kin}} \cot \left( \frac{\theta}{2} \right)
```

For greater than $90^{\circ}$

```math
\sigma_{\geq 90^{\circ}} = \pi b_{90^{\circ}}^{2} = \pi \left(\frac{Z_{\alpha}Z_{Pt}e^{2}}{8 \pi \epsilon_{0} E_{kin}} \right)^{2}
```

This is the Cross Section for 1 nucleus and the active area that will cause scatter.

```math
N = n \Delta A d
```

```math
n = \frac{\rho N_{A}}{M}
```

> |Quantity|Measurement|
> |-|-|
> |$N$|Number of Platinum Nuclei|
> |$n$|Number density of the Platinum nuclei|
> |$\rho$|Mass density|
> |$M$|Molar Mass|
> |$N_{A}$|Avogadro's number|

```math
f = \frac{\Delta A_{eff, \geq 90^{\circ}}}{\Delta A} = n d \sigma_{\geq 90^{\circ}}
```

## Size of a Nucleus

By increasing the kinetic energy of the particle we use to probe the nucleus, we can find smaller distances. Below a critical value. For the distance of closest approach $\delta$, the observed angular distribution $N(\theta)$ of scattered particles begins to deviate from the distribution calculated from a pure Coulomb potential. When simplified, $\delta_{N} \rightarrow R_{K}$ the nuclear radius.

At high angles/ energies, the distance of closest approach becomes small enough and the particle can interact with the nucleus via the strong nuclear force. This 'cliff' marks the threshold of the internal nuclear structure.

```math
R_{K} = r_{0}A^{\frac{1}{3}}
```

## Charge and Matter Density

The differential cross section for the elastic scattering of an electron from a nucleus with a finite charge distribution $\rho (r)$ is given by the scattering cross section from a point charge, corrected by a form factor

```math
\frac{d\sigma}{d \Omega} = \left(\frac{d\sigma}{d \Omega}\right)_{point} |F(\mathbf{q}^{2})|^{2}
```

Where $\mathbf{q} = \mathbf{P}_{f} - \mathbf{P}_{i}$, initial and final electron momenta. 

It describes how the spatial distribution of charge modifies the amplitude for an electron to scatter from the nucleus with momentum transfer $\mathbf{q}$

Using experimental data, the form factor can be determined and so, the charge density $\rho(r)$

## Fermi Distribution

Also known as the Woods-Saxon Potential

```math
\rho (r) = \frac{\rho (0)}{1 + \exp \left({\frac{r-R_{\frac{1}{2}}}{d}}\right)}
```

> |Quantity|Measurement|
> |-|-|
> |$\mathbf{q}$|Momentum transfer|
> |$\rho(r)$|Charge density|
> |$\rho(0)$|Central charge density|
> |$R_{\frac{1}{2}}$|Half-density radius|
> |$d$|Surface thickness of nucleus|
> |$R_{K}$|Hard sphere radius|
> |$r_{0}$|Radius of nucleon $\approx 1.2\text{fm}$|

Electron scattering experiment yielded:

- Charge density, proton distribution is approximately constant in the nuclear interior and falls rapidly to zero at the nuclear surface
- $R_{\frac{1}{2}} increases slowly with increasing mass number $A$ and is $\propto A^{\frac{1}{3}}$
- Thickness of $d$ is nearly the same for all nuclei
- $/rho(0) decreases slowly with increasing $A$, multiplying by $\frac{A}{Z}$ will find the same matter density in the nuclear interior for $\approx$ all nuclei
- If the nucleus is approximated as a homogoneously charged sphere, then $R_{K} = r_{0}A^{\frac{1}{3}}$

## Relativistic Kinematics

> |Quantity|Measurement|
> |-|-|
> |$m$|Invariant/rest/proper mass|
> |$E$|Energy|
> |$\mathbf{p}$|Momentum|
> |$c$|Speed of light|
> |$\gamma$|$\frac{1}{\sqrt{1- \beta^{2}}}$|
> |$\beta$|\frac{v}{c}|

This quantity is invariant, some particles may be massless

```math
m^{2}c^{2} = \frac{E^{2}}{c^{2}} - \mathbf{p}^{2}
```

Kinetic energy for a massive particle is

```math
T = E - E_{rest} = \gamma mc^{2} - mc^{2} = (\gamma -1)mc^{2}
```

```math
T = \frac{1}{2} mv^{2}
```

For low velocities this is valid where $\frac{T}{mc^{2}} \approx 0.05$ or $\gamma \approx 1.05$ and $\beta \approx 0.3$

## Conservation

### Conservation and Lorentz Invariance of Quantities

Electric charge, lepton number, baryon number, and lepton flavour are conserved and are Lorentz invariant.

The conservation of baryon number implies the conservation of nucleon number

### Conservation but Not Lorentz Invariant

Energy and momentum conservation laws hold true in all reference frames, values of $E$ and $\mathbf{p}$ can change between frames, they are not Lorentz invariant, but the equality itself is preserved

### Lorentz Invariant but Not Conserved

Mass is Lorentz invariant, consider decay or where rest energy is not conserved

### Neither Conserved nor Lorentz Invariant

Kinetic energy/ velocity, can be converted between rest energy

## Difference Table

$$
\begin{array}{|c|c|c|}
\hline
\text{} & \text{Lorentz Invariant} & \text{Not Lorentz Invariant} \\
\hline
\text{Conserved} & \text{Electric charge, lepton number,} \\ & \text{baryon number, and lepton flavour} & \text{Energy and momentum conservation laws} \\
\hline
\text{Not Conserved} & \text{Mass under decay or} \\ & \text{rest mass not conserved} & \text{Kinetic energy/ velocity,} \\ & &\text{can be converted between rest energy} \\
\hline
\end{array}
$$


