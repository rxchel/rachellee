---
layout: default
title: Electron-Molecule Scattering
permalink: /projects/electron-scattering/
---

# Electron-Molecule Scattering

**Computational Chemistry · Electron Scattering · Quantum Chemistry · HPC**

## Project Overview

This project investigates low-energy electron scattering from methane (CH₄)
using computational quantum chemistry and scattering theory. The goal was to
calculate electron-scattering cross sections and characterize features of the
scattering process, including Ramsauer-Townsend minima and resonance structures.

I used two independent computational approaches, **UKRmol+** and **ASTRA**, to
investigate the scattering problem and compare the resulting predictions.

---

## My Contributions

My work on this project spanned the setup, execution, analysis, and
interpretation of the scattering calculations.

### Electronic Structure and Model Preparation

I prepared the molecular electronic structure calculations required as input
for the scattering calculations, including molecular geometry optimization and
molecular orbital generation using **Psi4**.

I investigated different basis sets, symmetry settings, and active-space
parameters to establish computational models suitable for the scattering
calculations.

### UKRmol+ Scattering Calculations

I configured and ran electron-molecule scattering calculations using
**UKRmol+**, including the construction of the molecular target and continuum
basis and the setup of close-coupling calculations.

I performed calculations on a high-performance computing cluster and
troubleshot issues involving continuum basis construction, target-state
coupling, and calculation settings.

### ASTRA Scattering Calculations

I independently set up electron-scattering calculations using **ASTRA** and
used the results to provide a comparison with the UKRmol+ calculations.

This involved preparing the required input files, selecting appropriate
scattering-model parameters, running calculations on an HPC system, and
processing the resulting scattering data.

### Data Analysis and Benchmarking

I analyzed the calculated scattering cross sections as a function of incident
electron energy and identified characteristic features of the scattering
curves.

I compared the calculated results from UKRmol+ and ASTRA with literature
values to evaluate the ability of each computational approach to reproduce
experimentally and theoretically important scattering features.

---

## Computational Methods

### UKRmol+

UKRmol+ was used to perform electron-molecule scattering calculations within a
close-coupling framework. The calculations included a configuration-interaction
description of the molecular target together with a continuum representation
of the incoming electron.

### ASTRA

ASTRA was used as an independent approach to calculate electron-scattering
observables. Comparing the ASTRA and UKRmol+ calculations provided a way to
evaluate the effects of computational method, basis set, and model-space
choices on the predicted scattering behavior.

---

## Software & Technical Skills

**Scientific Software**

- UKRmol+
- ASTRA
- Psi4

**Programming & Data Analysis**

- Python
- Data visualization
- Numerical data analysis

**Computational Environment**

- Linux
- High-performance computing (HPC)
- Bash / command-line workflows

**Methods**

- Quantum chemistry
- Configuration interaction
- Close-coupling scattering calculations
- Electron-molecule scattering
- Computational benchmarking

---

## Results

The calculations produced electron-scattering cross sections as a function of
incident electron energy.

The calculated scattering curves reproduced important qualitative features of
the methane electron-scattering problem, including a Ramsauer-Townsend minimum
and resonance structures.

The results from the two computational approaches were compared with one
another and with values reported in the literature. This comparison provided
insight into how choices such as basis set, active space, target-state
representation, and scattering model affect the calculated results.

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

## What I Learned

This project gave me hands-on experience applying computational chemistry
methods to a challenging scattering problem and working with research software
on a high-performance computing system.

In particular, I developed experience with:

- Setting up and troubleshooting computational chemistry calculations
- Working with quantum chemistry and electron-scattering software
- Running scientific calculations on Linux/HPC systems
- Analyzing and visualizing numerical simulation data
- Comparing independent computational approaches
- Benchmarking computational results against literature values
- Communicating technical results through scientific writing and presentation

---

## Summary

This project combined quantum chemistry, scattering theory, scientific
programming, and high-performance computing to investigate electron-molecule
scattering from methane. The use of both UKRmol+ and ASTRA provided an
opportunity to compare computational approaches while developing practical
experience with the full workflow from molecular model preparation through
calculation, data analysis, and scientific communication.
