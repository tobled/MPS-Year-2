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
\frac{T_{\alpha}}{T_{D}} = \frac{m_{D}}{m_{\alpha}}, \quad T_{\alpha} + T_{D} = Q
```

So,

```math
T_{D} = Q \frac{m_{\alpha}}{m_{\alpha}+m_{D}}, \quad T_{\alpha} = Q \frac{m_{D}}{m_{\alpha}+m_{D}}
```

Typically, the $\alpha$ particle carries 98% of the Q value while the heavier daughter nucleus carries about 2%. Recoil energy is not negligible on orders of 100 keV which exceeds many atomic binding energies in solids. If the decay occurs near the surface of a source, the recoiling nucleus may also escape into the surrounding material.

### Gamow Theory

To explain the mechanism of $\alpha$ decay, it is proposed that the $\alpha$ particle is preformed inside the parent nucleus. It is formed when 2 protons and neutrons from their highest energy levels combine to form a quasi-bound state.

Inside a nucleus, the $\alpha$ particle experiences both the short-range attractive strong nuclear force and the long-range Coulomb repulsion from the daughter nucleus. At small seperations the strong force dominates which produces a potential well that confines the $\alpha$ particle. Beyond the surface, the strong force goes to 0 and only the Coulomb force remains, making a potential barrier

If the $\alpha$ particle and the daughter nucleus are just in contact then strong force falls to zero and contact distance $r$ is given as:

```math
r = R_{D} + R_{\alpha} = r_{0}\left(A^{\frac{1}{3}}_{D}+A^{\frac{1}{3}}_{\alpha}\right)
```

## Beta Decay

The most basic type of beta decay is the conversion of a neution into a proton ora proton into a neutron. Both $Z$ and $N$ change by one unit

```math
Z \rightarrow Z \pm 1 \qquad N \rightarrow N \mp 1
```

$A$ remains constant which allows for unstable nuclei to approach the stable isobar.

### The Neutrino

In the 1910's and 20's, the continuous distribution of the $\beta$ electrons were studied. With $\alpha$ decay, the emitted particles ave sharp, well-defined energies by the difference in energy between the initial and final states. This is not the case with $\beta$ decay as a spectrum was found with properties:

```math
0 \leq E_{\beta} \leq E_{max}
```

This concludes with the idea that there must be another particle emitted that carries away the missing energy and momentum.

> The neutrino will be treated as massless

### Beta Minus Decay

Neutron turns into a proton, emitting an electron and an antineutrino to balance the lepton nummber.

```math
n \rightarrow p + e^{-} + \bar{\nu_{e}}
```

In general:

```math
^{A}_{Z}X \rightarrow ^{A}_{Z+1}Y + e^{-} + \bar{\nu_{e}}
```

A free neutron can decay spontaneously unlike a proton because it has more mass than the decaying products

Q value interms of nuclear masses is

```math
Q_{\beta^{}-} = [M_{N}(A,Z) - M_{N}(A, Z+1)-m_{e}]c^{2}
```

Then converting to **_atomic masses_** $M(A,Z)$ related by:

```math
M(A,Z)c^{2} = M_{N}(A,Z)c^{2} + Zm_{e}c^{2} - \sum_{i=1}^{Z} B_{atom, \, i}
```

With $B_{atom, \, i}$ the individual electron binding enrgies, the Q-Value can be expressed as:

```math
Q_{\beta^{-}} = \left([M(A,Z) - Zm_{e}] - [M(A,Z+1) - (Z+1)m_{e}] - m_{e} \right) c^{2} + [\sum_{i=1}^{Z+1} B_{atom, \, i} - \sum_{i=1}^{Z} B_{atom, \, i}]
```

These binding energies are small and can be neglected

```math
Q_{\beta^{-}} = \left([M(A,Z) - Zm_{e}] - [M(A,Z+1) - (Z+1)m_{e}] - m_{e} \right) c^{2}
```

For $\beta^{-}$ decay, the electron masses cancel and lead to

```math
Q_{\beta^{-}} = [M(A,Z)-M(A,Z+1)]c^{2}
```

The released energy is shared between the electron and neutrino:

```math
Q_{\beta^{-}}=T_{e} + E_{\nu} \qquad (T_{e})_{max} = (E_{\nu})_{max} = Q_{\beta^{-}}
```

### Beta Plus Decay

In $\beta^{+}$ decay, a proton converts into a neutron emitting a positron and a neutrino:

```math
p \rightarrow n + e^{+} + \nu_{e}
```

A free proton cannot undergo this decay and is only possible if the resulting neutron can occupy a lower energy level than the original proton

In general:

```math
^{A}_{Z}X \rightarrow ^{A}_{Z-1}Y + e^{+} + \nu_{e}
```

When using atomic masses. the position mass does not cancel so the Q-value ignoring atomic binding energy differences is:

```math
Q_{\beta^{-}} = [M(A,Z) - M(A,Z-1)-2m_{e}]c^{2}
```

### Electron Capture

Electron capture happens when a proton coptures an inner shell electron

```math
pp + e^{-} \rightarrow n + \nu_{e}
```

In general:

```math
^{A}_{Z}X + e^{-} \rightarrow ^{A}_{Z_1}Y+\nu_{e}
```

The Q-value goes as follows:

```math
Q_{EC} = [M(A,Z) - M(A,Z-1)]c^{2} - B_{n}
```

```math
Q_{EC} = [M(A,Z) - M(A,Z-1)]c^{2}
```

> Q value must be positive, some nuclei undergo both beta plus and EC while others undergo EC exclusively if $Q_{EC} \geq 0$ and $Q_{\beta^{+}} < 0$

## Gamma Decay

Most $\beta$ and $\alpha$ decays leave the final nucleus in an excited state. These rapidly decay to the ground state through the emission of one or more $\gamma$ rays. A stationary excited mass will conserve momentum by recoiling in the opposite direction to the gamma ray such that:

```math
p_{R} + p_{\gamma} = 0 \quad \rightarrow \quad |p_{R}| = |p_{\gamma}|
```

Using the relationship that $E_{\gamma} = c p_{\gamma}$

```math
|p_{R}| = \frac{E_{\gamma}}{c}
```

Energy conservation tells us that:

```math
E_{i} = E_{f} + E_{\gamma} + T_{R} \quad \rightarrow \quad \Delta E = E_{i} - E_{f} = E_{\gamma} + \frac{E_{\gamma}^{2}}{2Mc^{2}}
```

Use the non-relatavistic approximation for the recoil since the nucleus has a large rest energy $(\Delta E << Mc^{2})$

```math
T_{R} = \frac{p_{R}^{2}}{2M} = \frac{E_{\gamma}^{2}}{2Mc^{2}}
```

```math
E_{\gamma} = Mc^{2} \left[\sqrt{1+\frac{2\Delta E}{Mc^{2}}} - 1\right]
```

$\Delta E$ is small so expand the square root:

```math
\sqrt{1+x} \approx 1 + \frac{x}{2} - \frac{x^{2}}{8} + ...
```

With only the first two non-zero terms:

```math
E_{\gamma} \approx \Delta E - \frac{(\Delta E)^{2}}{Mc^{2}}
```

The range of energies is between 1 and 100 eV recoils, for high-energy $\gamma$ rays, radiation damage may be observable

## Decay Rates

If there are many identical nuclei at $t=0$, let $N(t)$ denote the number of undecayed nuclei at time $t$ where $\lambda$ is the decay constant:

```math
\frac{dN}{dt} = -\lambda N
```

Separating the variables and integrating to get:

```math
N(t) = N(0)e^{-\lambda t}
```

Let the mean lifetime of unstable particles be $\tau$, weighted by the number of $\lambda N(t)$ of particles decaying within the interval $dt$:

```math
\tau = \frac{1}{N(0)} \int_{0}^{\infty} t \lambda N(t)dt
```

This evaluates as:

```math
\tau = \frac{1}{\lambda} \qquad \tau_{1/2} = \frac{\text{ln }2}{\lambda}
```

```math
\tau = \frac{1}{\lambda} = \frac{\tau_{1/2}}{\text{ln }2}
```

The number of decays per unit time (decay rate) is defined as the activity:

```math
A(t) = -\frac{dN}{dt} = \lambda N(t) = \frac{N(t)}{\tau}
```

> There will be random fluctuations which can be measured with the standard deviation, which for $\Delta N > 5$ can be approximated as $\sigma = \sqrt{\Delta N}$
>
> It is common to express the decay of an unstable partivle in terms of its decay width $\Gamma$ with units of energy: $\lambda = \frac{1}{\tau} = \frac{\Gamma}{\hbar}$

### Multi-Modal Decays

A radioactive nuclide can sometimes decay through more than one channel, each with its own decay constant. One parent nuclide can decay into several daughter nuclides each with partial decay constant $\lambda_{i}$

The total decay rate is the sum of the partial decay constants so that:

```math
N(t) = N(0)\prod_{i} e^{-\lambda_{i}t}=N(0)e^{-\sum_{i}\lambda_{i}t}
```

Half-life of the parent is therefore:

```math
\tau_{1/2} = \frac{\text{ln }2}{\sum_{i}\lambda_{i}}
```

The branching ratio $B_{j}$ is:

```math
B_{j} = \frac{\lambda_{j}}{\sum_{i}\lambda_{i}}
```

## Nuclear Reactions

A typical nuclear reaction can be expressed as:

```math
X + a \rightarrow Y + b
```

Where $a$ is the incoming projectile, $X$ is the target nucleus, and $Y$ and $b$ are the products

$$
X + a \rightarrow
\begin{cases}
  X + a & \text{elastic scattering} \\
  X^{*} + a & \text{inelastic scattering} \\
  Y + b & \text{nuclear transformation}
\end{cases}
$$

For elastic scattering, energy is retained in the COM system and the target nucleus $X$ remains unchanged. For inelastic scattering, the nucleus $X$ is excited to $X^{*}$

### Reaction Q-Value

Consider the reaction:

```math
X + a \rightarrow Y+b
```

The Q value is:

```math
Q = (m_{X} + m_{a} - m_{Y} - m_{b})c^{2}
```

The conservation of energy for rest and kinetic energies give:

```math
m_{X}c^{2} + m_{a}c^{2} + T_{X} + T_{a} = m_{Y}c^{2} + m_{b}c^{2} + T_{Y} + T_{b}
```

This allows the Q-value to be written like this:

```math
Q = (T_{Y} + T_{b}) - (T_{X} + T_{a})
```

Any chance in the kinetic energy of the reacting system must be balanced by an equal and opposite change in its rest energy.

The Q-Value may be positive, negative, or zero:

- If $Q > 0$, Exothermic reaction, rest energy is converted to kinetic energy of the final products
- If $Q < 0$, Endothermic reaction, kinetic energy must be supplied which is converted to additional rest energy
