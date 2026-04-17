# Macroscopic Dephasing in LMT Atom Interferometry from an Operational Coherence-Cell Bridge

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19186680.svg)](https://doi.org/10.5281/zenodo.19186680)

**Author:** Eric C. Thompson  
**Contact:** ethompson06@gmail.com  

**A Short Letter on the NDK Momentum-Quadratic Contrast Floor**

This repository contains the LaTeX manuscript and companion Python tools for a phenomenological bridge between the Null-Directional Kinematics (NDK) transport framework and Large Momentum Transfer (LMT) atom interferometry.

## Overview
A central open question in macroscopic quantum mechanics is whether contrast loss in LMT atom interferometry is fully reducible to environmental and technical noise, or whether an irreducible geometric floor appears once momentum separation and interrogation time become sufficiently large.

This Letter develops a forward prediction based on a finite-throughput transport picture of the directional vacuum. In its current form, the paper replaces the earlier fixed-cell language with a **closure-informed operational coherence-cell bridge**, in which the transport burden is inherited from the reduced NDK Fisher transport sector while the laboratory-side coherence scale is encoded through an operational pre-split coherence-cell prescription.

The resulting leading-order residual dephasing law has characteristic scaling

`D_pred ∝ T * n^2 * k_eff^2`

with normalization controlled by the ratio of the interferometric coherence-support width to the pre-split coherence length of the atomic source.

The normalization is anchored to the cosmologically calibrated directional-strain threshold (`I*/A ≈ 3.28`) adopted from the broader NDK program, while recent action-scale closure work sharpens the upstream normalization by isolating the primitive cell as the unique carrier of the absolute action scale. In that sense, the remaining phenomenology resides in the laboratory transfer bridge rather than in an arbitrary ultraviolet normalization choice.

## Experimental Falsification Target
The operational coherence-cell bridge establishes a concrete forecast for long-baseline atom interferometers:

- **Current technology (`n ~ 10^2`)**: predicted intrinsic residual dephasing remains strongly suppressed and parametrically below the relevant sensitivity window.
- **Long-time MAGIS-like regimes (`n ~ 10^3`)**: the residual can move into the sub-percent sensitivity window and, for broader representative coherence-support widths, approach the `10^-3` contrast-loss benchmark.

If future `n ~ 10^3` LMT interferometers fail to exhibit a residual contrast-loss component with leading quadratic dependence on LMT order `n` at fixed interrogation time `T`, then the operational coherence-cell bridge proposed here is falsified as the laboratory realization of the NDK transport prediction.

## Repository Contents

- **`paper.tex`**: complete LaTeX source for the Short Letter.
- **`ndk_lmt_calculator.py`**: forward-model calculator for evaluating transport burden, residual dephasing, visibility loss, and coherence-scale requirements for specific experimental sequences.
- **`ndk_scaling_plot.py`**: focused scaling-plot script for the operational coherence-cell bridge, including the long-time thermal operating-point figure and representative width-sensitivity band.

## Citation
If you use this code or reference the framework, please cite the corresponding Zenodo record:

```bibtex
@misc{thompson2026dephasing,
  author    = {Thompson, Eric C.},
  title     = {Macroscopic Dephasing in LMT Atom Interferometry from an Operational Coherence-Cell Bridge: A Short Letter on the NDK Momentum-Quadratic Contrast Floor},
  year      = {2026},
  publisher = {Zenodo},
  doi       = {10.5281/zenodo.19186680},
  url       = {https://doi.org/10.5281/zenodo.19186680}
}
