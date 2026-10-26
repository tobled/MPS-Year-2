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

> | Symbol       | Measure                            | Unit | SI                                       |
> | ------------ | ---------------------------------- | ---- | ---------------------------------------- |
> | $\sigma$     | Cross Section                      | $1b$ | $10^{-28}\mathrm{m^{2}}$                 |
> | $\phi$       | Flux of Incident Beam              | -    | $\text{in particles} \cdot m^{-2}s^{-1}$ |
> | $N_{target}$ | No. of target particles            | -    | -                                        |
> | $R$          | Rate of observed scattering events | -    | $s^{-1}$                                 |

```math
R = \phi N_{target} \sigma
```

Cross section is the effective area taken out of the incoming beam of particles by each particle in the target. The cross section for scattering into an angle between $\theta$ and $\theta + d\theta$ is just the area of the ring. Using the integral to find the cross section for angle $\geq \theta$

```math
\sigma = \int_{0}^{b(\theta)} 2 \pi b \,db = \pi b^{2}(\theta)
```

## Alpha Particle Scattering

Take a setup that uses an alpha particle beam directed at a platinum foil.

> | Quantity  | Unit                           |
> | --------- | ------------------------------ |
> | $E_{kin}$ | $5\, \mathrm{MeV}$             |
> | $d$       | $1.2 \times 10^{-4} \text{cm}$ |

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

> | Quantity | Measurement                           |
> | -------- | ------------------------------------- |
> | $N$      | Number of Platinum Nuclei             |
> | $n$      | Number density of the Platinum nuclei |
> | $\rho$   | Mass density                          |
> | $M$      | Molar Mass                            |
> | $N_{A}$  | Avogadro's number                     |

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

> | Quantity          | Measurement                              |
> | ----------------- | ---------------------------------------- |
> | $\mathbf{q}$      | Momentum transfer                        |
> | $\rho(r)$         | Charge density                           |
> | $\rho(0)$         | Central charge density                   |
> | $R_{\frac{1}{2}}$ | Half-density radius                      |
> | $d$               | Surface thickness of nucleus             |
> | $R_{K}$           | Hard sphere radius                       |
> | $r_{0}$           | Radius of nucleon $\approx 1.2\text{fm}$ |

Electron scattering experiment yielded:

- Charge density, proton distribution is approximately constant in the nuclear interior and falls rapidly to zero at the nuclear surface
- $R_{\frac{1}{2}} increases slowly with increasing mass number $A$ and is $\propto A^{\frac{1}{3}}$
- Thickness of $d$ is nearly the same for all nuclei
- $/rho(0) decreases slowly with increasing $A$, multiplying by $\frac{A}{Z}$ will find the same matter density in the nuclear interior for $\approx$ all nuclei
- If the nucleus is approximated as a homogoneously charged sphere, then $R_{K} = r_{0}A^{\frac{1}{3}}$

## Relativistic Kinematics

> | Quantity     | Measurement                     |
> | ------------ | ------------------------------- |
> | $m$          | Invariant/rest/proper mass      |
> | $E$          | Energy                          |
> | $\mathbf{p}$ | Momentum                        |
> | $c$          | Speed of light                  |
> | $\gamma$     | $\frac{1}{\sqrt{1- \beta^{2}}}$ |
> | $\beta$      | \frac{v}{c}                     |

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

## Nuclear Binding Energy and Mass Defect

> | Quantity       | Measurement                           |
> | -------------- | ------------------------------------- |
> | $E_{N}$        | Energy of nucleus                     |
> | $E\_{B}        | Nuclera binding energy                |
> | $E_{0}$        | Rest energy from Protons and Neutrons |
> | $A$            | Mass Number                           |
> | $Z$            | Proton Number                         |
> | $m_{x}$        | Mass of x                             |
> | $N$            | Neutron Number                        |
> | $\Delta M_{N}$ | Nuclear mass defect                   |

Consider a system of protons and neutrons and the nucleus at rest

```math
E_{0}(A,Z) = (Zm_{p} + (A-Z)m_{n})c^{2} = (Zm_{p}+Nm_{n})c^{2}
```

For free nucleons

```math
E_{N}(A,Z) = M_{N}(A,Z)c^{2}
```

```math
E_{N}(A,Z) = E_{0}(A,Z) - E_{B}(A,Z)
```

Becomes:

```math
M_{N}(A,Z)c^{2} = (Zm_{p} + Nm_{n})c^{2} - E_{B}(A,Z)
```

```math
M_{N}(A,Z) = (Zm_{p} + Nm_{n}) - \frac{E_{B}(A,Z)}{c^{2}}
```

The mass defect is defined as

```math
\Delta M_{N}(A,Z) = (Zm_{p} + Nm_{n}) - M_{N}(A,Z) = \frac{E_{B}(A,Z)}{c^{2}}
```

```math
\Delta M_{N}(A,Z) = ZM_{H} + Nm_{n} - M(A,Z) = \frac{E_{B}(A,Z)}{c^{2}}
```

> | Quantity | Measurement                          |
> | -------- | ------------------------------------ |
> | $M_{H}$  | Atomic mass of neutral hydrogen atom |
> | $1 u$    | $931.49$ $MeV/c^{2}$                 |

## Nuclear Stability

For small $Z$, stable nuclei have roughly the same number of protons and neutrons $(Z \approx N)$. For large nuclei, stable isotopes have $Z < N$

There also seems to be a pattern of even $Z$ and even $N$ for stable nuclei.

## The Liquid Drop Model and Semi-Empirical Mass Formula

For all but the lightest nuclei, the binding energy can be reproduced by a formula that uses the idea that the nucleus can be treated as a liquid drop of nucleons. It uses the these two properties:

- Interior mass densities are approximately constant
- Total binding energies are approximately proportional to their masses $\frac{B}{A} \approx \text{const.}$

These can be compared with the macroscopic drops of incompressible liquid:

- Interior denisties are the same
- Heats of vaporization are proportional to their masses

The heat of vapourization is the energy required to disperse the drop into its constituent molecules much like the binding energy of the nucleus

We can start with this equation to develop a semi-empirical mass formula by including terms that account for nuclear properties that may be quantum-mechanical rather than classical

```math
M_{N}(A,Z) = (Zm_{p} + Nm_{n}) - \frac{E_{B}(A,Z)}{c^{2}}
```

## The Terms

Coeffiecients of the semi-empirical mass formula

> | Term      | Quantity     | Value $(MeV)$ |
> | --------- | ------------ | ------------- |
> | Volume    | $a_{V}$      | $15.8$        |
> | Surface   | $a_{S}$      | $18.3$        |
> | Coulomb   | $a_{C}$      | $0.714$       |
> | Asymmetry | $a_{C}$      | $23.2$        |
> | Pairing   | $a_{\delta}$ | $12.0$        |

### Volume Term

The force that keeps the nucleus together. The short range of the nuclear force implies that each nucleon interacts only with its nearest neighbours. $K$ is the number of neighbouring nucleons where the contribution is $KA \propto A$

```math
E_{volume} = a_{V}A
```

### Surface Term

Surface nucleons experience fewer attractive interactions that those in the interior

```math
E_{surface} = - a_{S}A^{\frac{2}{3}}
```

### Coulomb Term

Protons have a replusive Coulomb force that reduces binding energy, happens between pairs

```math
E_{Coulomb} = -a_{C} \frac{Z(Z-1)}{A^{\frac{1}{3}}}
```

### Asymmetry Term

Low mass number stable nuclei have equal numbers of protons fand neutrons

```math
E_{asymmetry} = -a_{A} \frac{(N-Z)^{2}}{A}
```

### Pairing Term

$$ \delta(A,Z) = \begin{cases} +\Delta, & \text{even-even nuclei,} \\ 0, & \text{odd A,} \\ +\Delta, & \text{odd-odd nuclei,} \end{cases} $$

Where

```math
\Delta = a_{\delta} A^{-\frac{1}{2}}
```

## Formula 1

```math
E_{B}(A,Z) = a_{V}A - a_{S}A\frac{2}{3} - a_{C}\frac{Z(Z-1)}{A^{\frac{1}{3}}} - a_{A}\frac{(N-Z)^{2}}{A} + \delta(A,Z)
```

## Fermi Gas Model

Assume that nucleons in the nucleus move in an attractive average potential that represents the net effect of its interactions with all other nucleons. This potential can be modelled by a 3D finite square well with a radius slightly larger than the nuclear radius

Fermions obey the Pauli exclusion principle, the nucleus can be treated as two independant Fermi gases one for protons and one for neutrons

For small Z, the Coulomb repulsion between protons can be neglected and the energy levels of the proton and neutron systems are the same.

## Decay Q-Value

Conservation of energy for a general decay implies:

```math
m_{i}c^{2} + T_{i} = \sum m_{f}c^{2} + \sum T_{f}
```

```math
(m_{i}-\sum m_{f})c^{2} = \sum T_{f}-T{i}
```

Difference between the rest energies of the initial and final particles is called the Q-value

```math
Q = (m_{i}-\sum m_{f})c^{2}
```

```math
Q = \sum T_{f} - T_{i}
```

Q-value is the excess kinetic energy provided to the decay products, a spontaneous decay can only happen if $Q \geq 0$. Q may be quantified in MeV

## Alpha Decay

Alpha decay is an emission of an $\alpha$ particle which is a He nucleus

```math
_{Z}^{A}P \rightarrow _{Z-2}^{A-4}D + \alpha
```

### Alpha Decay Example

```math
Q = (m_{P}-m_{D}-m_{\alpha})c^{2}
```

If at rest:

```math
Q = (m_{P}-m_{D}-m_{\alpha})c^{2} = T_{D}+T_{\alpha}
```

Conservation of momentum requires that $D$ and $\alpha$ move with equal and opposite momenta

Alpha decays typically release energies of order 5 MeV which is much smaller than the rest energies of the particles where $T \ll mc^{2}$ we may safely use the non-relatavistic approximation.

```math
\frac{T_{D}}{T_{\alpha}} = \frac{m_{D}}{m_{\alpha}}, \, T_{\alpha} + T_{D} = Q
```

So,

```math
T_{D} = Q \frac{m_{\alpha}}{m_{\alpha}+m_{D}}, \, T_{\alpha} = Q \frac{m_{D}}{m_{\alpha}+m_{D}}
```

Typically, the $\alpha$ particle carries 98% of the Q value while the heavier daughter nucleus carries about 2%. Recoil energy is not negligible on orders of 100 keV which exceeds many atomic binding energies in solids. If the decay occurs near the surface of a source, the recoiling nucleus may also escape into the surrounding material.
