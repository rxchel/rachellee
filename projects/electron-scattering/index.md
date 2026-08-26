---
layout: default
title: Electron-Molecule Scattering
permalink: /projects/electron-scattering/
---

# _Ab Initio_ Electron-Molecule Scattering Calculations for Methane Using UKRMol+ and ASTRA

**Computational Chemistry · Quantum Scattering · Scientific Computing · Physical Chemistry**

## Project Overview

This project investigated low-energy electron scattering from methane (CH₄)
using computational quantum chemistry and scattering theory.

The objective was to calculate electron-scattering cross sections and identify
important features of the scattering process, including the
Ramsauer-Townsend (R-T) minimum and resonance structures.

I investigated the scattering problem using two computational approaches,
**UKRmol+** and **ASTRA**, and compared the resulting calculations with one
another and with literature values.

---

## My Contributions

I worked across the computational workflow, from preparing the molecular model
and configuring scattering calculations to running simulations on a
high-performance computing cluster and analyzing the resulting data.

### Molecular Model Preparation

I prepared the molecular electronic structure used as the basis for the
scattering calculations.

This included working with **Psi4** to generate molecular orbitals and
investigating computational parameters including molecular symmetry, basis
sets, and active-space settings.

### UKRmol+ Calculations

I set up and ran electron-molecule scattering calculations using
**UKRmol+** and its close-coupling framework.

I worked with the molecular target representation, continuum basis, target
states, and scattering-model parameters. I also diagnosed and troubleshot
issues encountered during calculation setup and execution.

### ASTRA Calculations

I independently configured and ran scattering calculations using **ASTRA**.

I investigated how choices such as basis set, active-space size, angular
momentum, and target-state representation affected the calculations and used
ASTRA as an independent computational approach for comparison with UKRmol+.

### HPC Computing & Troubleshooting

The calculations were performed on a Linux-based high-performance computing
cluster.

I developed experience working with command-line workflows, managing
computational jobs, interpreting program output and error messages, and
troubleshooting calculations that did not initially run as expected.

### Data Analysis

I processed and analyzed calculated electron-scattering cross sections as a
function of incident electron energy using **Python**.

I compared results from UKRmol+ and ASTRA and benchmarked the calculations
against literature values to evaluate the calculated scattering behavior.

---

## Computational Methods

### UKRmol+

UKRmol+ was used to perform electron-molecule scattering calculations within
a close-coupling framework.

The calculations combined a quantum-chemical description of the molecular
target with a representation of the incident electron and were used to
calculate scattering observables.

### ASTRA

ASTRA was used as an independent computational approach to calculate
electron-scattering observables.

Using both UKRmol+ and ASTRA allowed me to investigate how computational
methodology and model parameters influence the calculated scattering results.

---

## Tools & Skills

**Quantum Chemistry**

- UKRmol+
- ASTRA
- Psi4
- Configuration-interaction calculations
- Close-coupling scattering methods

**Programming & Data Analysis**

- Python
- Numerical data analysis
- Scientific visualization

**Computational Environment**

- Linux
- High-performance computing
- Command-line workflows
- Python notebooks

---

## Results

The calculations produced electron-scattering cross sections as a function of
incident electron energy.

Both computational approaches captured important features of the methane
electron-scattering problem, including a Ramsauer-Townsend minimum and
resonance structures.

The calculated results were compared between UKRmol+ and ASTRA and benchmarked
against literature values.

### Molecular Geometry

![Methane molecular geometry]({{ site.baseurl }}/assets/images/electron-scattering/CH4-geo-opt-D2.png)

*Optimized CH₄ molecular geometry used in the scattering calculations.*

![Electron-molecule scattering cross section]({{ site.baseurl }}/assets/images/electron-scattering/image18.png)

*e-CH₄ scattering cross sections.*

---

## Deliverables

### Presentation

[View the project presentation (PDF)](https://rxchel.github.io/rachellee/assets/files/electron-scattering/presentation.pdf)

### Report

[View the project report (PDF)](https://rxchel.github.io/rachellee/assets/files/electron-scattering/report.pdf)

---

## Project Takeaways

This project gave me experience with the end-to-end workflow of a
computational research project:

**molecular model preparation → computational setup → HPC calculations →
troubleshooting → data analysis → benchmarking → scientific communication**

Through this work, I developed practical experience with computational
quantum chemistry, electron-molecule scattering, scientific programming,
high-performance computing, and communicating technical results.
