<h1 align="center">Junquan Su</h1>

<p align="center">
  <b>PhD Student in Astronomy</b><br>
  Department of Astronomy, Tsinghua University
</p>

<p align="center">
  <a href="#research-interests">Research Interests</a> ·
  <a href="#publications">Publications</a> ·
  <a href="#numerical-tools">Numerical Tools</a> ·
  <a href="#education">Education</a> ·
  <a href="#contact">Contact</a>
</p>

---

## Research Interests

<p align="center">
  <b>Gravitational Wave Physics</b> &nbsp;·&nbsp; <b>Black hole perturbation theory</b>
</p>

---

## Publications

### Decomposition of the Schwarzschild Green's function

**Junquan Su**, Neev Khera, Marc Casals, Sizheng Ma, Abhishek Chowdhuri, and Huan Yang  
*Physical Review D* **113**, 104013 (2026)

[Journal](https://link.aps.org/doi/10.1103/3n8r-8kbb) · [Data](https://github.com/JunquanSu/Schwarzschild_Greens_Function_Decomposition_Data)

<details>
<summary><b>BibTeX</b></summary>

```bibtex
@article{3n8r-8kbb,
  title = {Decomposition of the Schwarzschild Green's function},
  author = {Su, Junquan and Khera, Neev and Casals, Marc and Ma, Sizheng and Chowdhuri, Abhishek and Yang, Huan},
  journal = {Phys. Rev. D},
  volume = {113},
  issue = {10},
  pages = {104013},
  numpages = {12},
  year = {2026},
  month = {May},
  publisher = {American Physical Society},
  doi = {10.1103/3n8r-8kbb},
  url = {https://link.aps.org/doi/10.1103/3n8r-8kbb}
}
```

</details>

<br>

### Gravitational Waves from Green's Function Decomposition for a Kerr Black Hole: I. Equatorial ISCO Plunge

**Junquan Su**, Neev Khera, Abhishek Chowdhuri, Marc Casals, and Huan Yang  
arXiv:2608.17943 [gr-qc] (2026)

[arXiv](https://arxiv.org/abs/2608.17943)

<details>
<summary><b>BibTeX</b></summary>

```bibtex
@article{Su:2026gmp,
    author = "Su, Junquan and Khera, Neev and Chowdhuri, Abhishek and Casals, Marc and Yang, Huan",
    title = "{Gravitational Waves from Green's Function Decomposition for a Kerr black hole: I. Equatorial ISCO Plunge}",
    eprint = "2608.17943",
    archivePrefix = "arXiv",
    primaryClass = "gr-qc",
    month = "8",
    year = "2026"
}
```

</details>

---

## Numerical Tools

The calculations in these works rely on a set of in-house numerical tools developed for black-hole perturbation theory. These currently include both **frequency-domain homogeneous solvers** and a **time-domain Teukolsky solver**.

### Frequency-domain homogeneous solvers

We have developed homogeneous solvers for the **Regge–Wheeler–Zerilli**, **Teukolsky**, and **Sasaki–Nakamura** equations. These solvers are designed to provide reliable radial solutions and asymptotic amplitudes over a relatively large parameter space, with particular emphasis on regimes involving large complex frequencies. For the Teukolsky equation, our frequency-domain suite also solves the **angular Teukolsky equation**, providing the corresponding angular solutions and separation eigenvalues, including at complex frequencies.

Considerable attention has been paid to numerical stability and reliability throughout the complex-frequency plane while retaining computational efficiency suitable for large-scale calculations.

In our tests, we have encountered many subtle but important theoretical issues in some currently available public implementations when they are applied at complex frequencies. In particular, some tools available through the [Black Hole Perturbation Toolkit](https://bhptoolkit.org/index.html) can exhibit inaccuracies in parts of the complex-frequency plane that may be difficult to detect in standard real-frequency calculations. We have also found that `GeneralizedSasakiNakamura.jl` becomes unreliable in regions of the $\omega$-plane close to the imaginary axis, and that at complex frequencies it may return incorrect radial solutions as well as incorrect angular solutions.

These observations motivated the development of our own independent numerical infrastructure, with an emphasis on robustness across the complex-frequency plane.

For practical reasons, the source code for these frequency-domain solvers will not be made public in the near term. Researchers interested in using the codes or comparing numerical results are welcome to contact me by email.

### Time-domain Teukolsky solver

We have also developed an independent **time-domain solver for the Teukolsky equation in horizon-penetrating, hyperboloidally compactified (HPHC) coordinates** which works on Nvidia GPUs. The formulation evolves the spin- $s$ Teukolsky equation on a compactified domain extending from the black-hole horizon to future null infinity $\mathcal{I}^{+}$, allowing the retarded waveform to be extracted directly at null infinity without an additional large-radius extrapolation.

For Kerr spacetime, the azimuthal dependence is decomposed into $m$-modes and the remaining system is evolved in $2+1$ dimensions. The implementation supports localized source profiles and has been used as an independent time-domain benchmark for our frequency-domain Green's-function calculations. In particular, in our Kerr Green's-function decomposition work, it was used to compare the directly evolved waveform at $\mathcal{I}^{+}$ against the waveform reconstructed from the direct and quasinormal-mode contributions.

A technical description of the current implementation can be found in **Appendix D** of:

> J. Su, N. Khera, A. Chowdhuri, M. Casals, and H. Yang,  
> *Gravitational Waves from Green's Function Decomposition for a Kerr Black Hole: I. Equatorial ISCO Plunge*,  
> [arXiv:2608.17943](https://arxiv.org/abs/2608.17943).

The time-domain solver is still being packaged and developed into a more reusable numerical tool, and we expect to use and extend it in future work. It will therefore not be publicly released in the near term. Depending on the progress of code maintenance, documentation, and packaging, we expect to make it semi-available on a request basis at a later stage. Once the code reaches that stage, researchers interested in using it will be welcome to contact me by email, in the same manner as for the frequency-domain solvers.

---

## Education

- 2025-    , Department of Astronomy, Tsinghua University, PhD Student
- 2022-2025, Department of Physics, School of Physics and Astronomy / TianQin Research Center for Gravitational Physics, Sun Yat-sen University, Undergraduate Student
- 2021-2022, Institut Franco-Chinois de l'Energie Nucléaire, Sun Yat-sen University, Undergraduate Student
- 2018-2021，South China Normal University High School
- 2015-2018, Guangzhou No.97 Middle School

---
