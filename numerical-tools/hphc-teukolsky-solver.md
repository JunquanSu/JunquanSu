<p align="center">
  <a href="../README.md">← Back to profile</a>
</p>

<h1 align="center">HPHC Time-Domain Teukolsky Solver</h1>

<p align="center">
  <b>Horizon-Penetrating Hyperboloidally Compactified Teukolsky Evolution</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/domain-time--domain-informational">
  <img src="https://img.shields.io/badge/coordinates-HPHC-informational">
  <img src="https://img.shields.io/badge/GPU-NVIDIA-informational">
</p>

---

## Overview

We have developed an independent **time-domain solver for the Teukolsky equation in horizon-penetrating, hyperboloidally compactified (HPHC) coordinates**.

The formulation evolves the spin-$s$ Teukolsky equation on a compactified domain extending from the black-hole horizon to future null infinity $\mathcal{I}^{+}$, allowing the retarded waveform to be extracted directly at null infinity without an additional large-radius extrapolation.

## Features

- Horizon-penetrating hyperboloidal formulation
- Direct waveform extraction at future null infinity $\mathcal{I}^{+}$
- Kerr spacetime evolution
- $m$-mode decomposition
- $2+1$ dimensional evolution
- GPU acceleration using NVIDIA GPUs
- Localized source profiles

## Applications

The solver has been used as an independent time-domain benchmark for our frequency-domain Green's-function calculations.

In our Kerr Green's-function decomposition work, it was used to compare the directly evolved waveform at $\mathcal{I}^{+}$ against the waveform reconstructed from the direct and quasinormal-mode contributions.

A technical description of the current implementation can be found in **Appendix D** of:

> J. Su, N. Khera, A. Chowdhuri, M. Casals, and H. Yang,  
> *Gravitational Waves from Green's Function Decomposition for a Kerr Black Hole: I. Equatorial ISCO Plunge*,  
> [arXiv:2608.17943](https://arxiv.org/abs/2608.17943).

## Availability

The time-domain solver is still being packaged and developed into a more reusable numerical tool, and we expect to use and extend it in future work.

It will therefore not be publicly released in the near term. Depending on the progress of code maintenance, documentation, and packaging, we expect to make it semi-available on a request basis at a later stage.

Researchers interested in using the solver will be welcome to contact me by email once the code reaches that stage.

---

<p align="center">
  <a href="../README.md">← Back to Junquan Su's profile</a>
</p>
