# Macroscopic Dephasing in LMT Atom Interferometry from a Fixed-Cell Transport Model

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19186681.svg)](https://doi.org/10.5281/zenodo.19186681)

**Author:** Eric Cole Thompson  
**Contact:** ethompson06@gmail.com  

**A Short Letter on the NDK Momentum-Quadratic Contrast Floor**

This repository contains the LaTeX manuscript and companion Python tools for a phenomenological bridge between the Null-Directional Kinematics (NDK) transport framework and Large Momentum Transfer (LMT) atom interferometry.

## Overview
A central open question in macroscopic quantum mechanics is whether contrast loss in LMT atom interferometry is fully reducible to environmental and technical noise, or whether an irreducible geometric floor appears at extreme momentum separations.

This Letter develops a forward prediction based on a finite-throughput transport picture of the directional vacuum. Using a fixed-cell ansatz—where the operational coherence cell is set by the pre-split thermodynamic preparation of the source and subsequently stressed by kinematic transport—the framework predicts a residual dephasing law with leading scaling

$D_{\mathrm{pred}} \propto T n^2 k_{\rm eff}^2$

The normalization is anchored to the cosmologically calibrated directional-strain threshold ($\mathcal{I}_*/A \approx 3.28$) adopted from the NDK supermassive black hole saturation analysis, enforcing a single benchmark across scales without laboratory parameter retuning.

## Experimental Falsification Target
The fixed-cell bridge establishes a concrete forecast for long-baseline atom interferometers:

- **Current technology ($n \sim 10^2$):** predicted intrinsic substrate dephasing remains strongly suppressed and parametrically below standard environmental noise.
- **MAGIS-like architectures ($n \sim 10^3$):** the accumulated kinematic burden enters the 1% to few-percent dephasing window.

If future $n \sim 10^3$ LMT interferometers fail to observe a residual contrast-loss component with leading quadratic dependence on LMT order $n$ at fixed interrogation time $T$, then the fixed-cell NDK bridge proposed here is falsified.

## Repository Contents

- **`paper.tex`**: complete LaTeX source for the Short Letter.
- **`ndk_lmt_calculator.py`**: forward-model calculator for estimating irreducible stochastic phase diffusion for specific experimental sequences.
- **`ndk_scaling_plot.py`**: scaling-plot script that sweeps the microscopic bridge variables and generates the interquartile dephasing bands showing the $n^2$ LMT contrast floor.

## Citation
If you use this code or reference the framework, please cite the corresponding Zenodo record:

```bibtex
@misc{thompson2026dephasing,
  author    = {Thompson, Eric Cole},
  title     = {Macroscopic Dephasing in LMT Atom Interferometry from a Fixed-Cell Transport Model: A Short Letter on the NDK Momentum-Quadratic Contrast Floor},
  year      = {2026},
  publisher = {Zenodo},
  doi       = {10.5281/zenodo.19186681},
  url       = {https://doi.org/10.5281/zenodo.19186681}
}
