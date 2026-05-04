# TMB_OX Microfluidic Biosensor Modeling

**Athena Antippas**  
Applied Mathematics, Middlebury College — Spring 2026  
Research conducted in collaboration with the Rahn Lab,
Middlebury College Department of Chemistry

---

## Overview

This repository contains the code appendix for the senior capstone project
*Modeling Fluid Dynamics of Oxidized 3,3',5,5' Tetramethylbenzidine (TMB_OX)
in a Microfluidic Biosensor*, completed for the Applied Mathematics major at
Middlebury College.

The project models reaction-advection-diffusion dynamics of TMB_OX in a microfluidic
electrochemical biosensor using analytical PDE solutions, with the goal of
optimizing incubation step timing to maximize signal and improve biosensor
sensitivity for cancer biomarker detection.

## Contents

- `AppendixB.ipynb` — Jupyter notebook reproducing Figures 5–13 from the paper

## Requirements

Python 3.x with the following packages:

```text
numpy
scipy
matplotlib
```

Install with:

```bash
pip install numpy scipy matplotlib
```

## Usage

Open `AppendixB.ipynb` in Jupyter and run all cells from **top to bottom**
in a single session. The notebook is organized as follows:

1. Imports
2. Formatting
3. Global Parameters (device constants matching Tables 1 and 2 in the paper)
4. Solver Functions (shared, Case 1, heatmap, and Case 2)
5. Figures 5–13, one labeled section per figure

Figures can be saved as PDFs by uncommenting the `plt.savefig(...)` line
at the end of each figure's cell.

> **Note:** Figures 9 and 10 (heatmaps) use a coarser spatial grid
> (`Nx = 150`) and a simplified sensing radius (`L_sens ~ cm`) for
> computational efficiency. The full-resolution grid (`Nx = 300`) is
> used for all other figures.

## Acknowledgments

Thank you to the Rahn Lab at Middlebury College Department of Chemistry
for providing the experimental context and device parameters that motivated
this work, and to the Middlebury Department of Mathematics for their
support throughout.