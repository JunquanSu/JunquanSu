<p align="center">
  <a href="../README.md">← Back to profile</a>
</p>

<h1 align="center">Frequency-Domain Solvers</h1>

<p align="center">
  <b>Regge–Wheeler–Zerilli · Teukolsky · Sasaki–Nakamura</b><br>
  Radial and angular black-hole perturbation solvers with complex-frequency support
</p>

<p align="center">
  <img src="https://img.shields.io/badge/domain-frequency--domain-informational" alt="frequency-domain">
  <img src="https://img.shields.io/badge/frequency-complex%20%CF%89-informational" alt="complex omega">
  <img src="https://img.shields.io/badge/Teukolsky-radial%20%2B%20angular-informational" alt="radial and angular Teukolsky">
</p>

---

## Overview

We have developed homogeneous solvers for the **Regge–Wheeler–Zerilli**, **Teukolsky**, and **Sasaki–Nakamura** equations. These solvers are designed to provide reliable radial solutions and asymptotic amplitudes over a relatively large parameter space, with particular emphasis on regimes involving large complex frequencies.

For the Teukolsky equation, our frequency-domain suite also solves the **angular Teukolsky equation**, providing the corresponding angular solutions and separation eigenvalues, including at complex frequencies.

## Capabilities

- Homogeneous **Regge–Wheeler–Zerilli** radial solutions
- Homogeneous **Teukolsky** radial solutions
- Homogeneous **Sasaki–Nakamura** radial solutions
- **Angular Teukolsky equation** solutions
- Separation eigenvalues
- Asymptotic amplitudes
- Calculations at **complex frequencies**, including regimes with relatively large complex frequency

## Numerical reliability

Considerable attention has been paid to numerical stability and reliability throughout the complex-frequency plane while retaining computational efficiency suitable for large-scale calculations.

In our tests, we have encountered many subtle but important theoretical issues in some currently available public implementations when they are applied at complex frequencies. In particular, some tools available through the [Black Hole Perturbation Toolkit](https://bhptoolkit.org/index.html) can exhibit inaccuracies in parts of the complex-frequency plane that may be difficult to detect in standard real-frequency calculations. We have also found that `GeneralizedSasakiNakamura.jl` becomes unreliable in regions of the $\omega$-plane close to the imaginary axis, and that at complex frequencies it may return incorrect radial solutions as well as incorrect angular solutions.

These observations motivated the development of our own independent numerical infrastructure, with an emphasis on robustness across the complex-frequency plane.

## Availability

For practical reasons, the source code for these frequency-domain solvers will not be made public in the near term. Researchers interested in using the codes or comparing numerical results are welcome to contact me by email.

---

<p align="center">
  <a href="../README.md">← Back to Junquan Su's profile</a>
</p>
