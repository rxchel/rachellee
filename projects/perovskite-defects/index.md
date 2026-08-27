---
layout: default
title: Perovskite Defects
permalink: /projects/perovskite-defects/
---

# Investigating the Defect Behavior and Electronic Properties of Formamidinium Lead Bromide Perovskite through Machine Learned Interatomic Potentials

**Computational Chemistry · Machine Learning · Molecular Dynamics · High Performance Computing**

![MLIP simulation of a FAPbBr₃ system containing a Schottky defect]({{ site.baseurl }}/assets/images/perovskite-defects/Model2train0-Schottky600.gif)

*MLIP simulation of a FAPbBr₃ system containing a Schottky defect.*

## Project Overview

This project investigated how **point defects affect the structural and electronic properties of formamidinium lead bromide (FAPbBr₃) perovskites**, a class of semiconductor materials with promising applications in optoelectronic devices.

FAPbBr₃ is of interest for applications including light-emitting diodes, photoelectrodes, and solar fuel cells, but defects within the crystal can significantly influence its electronic properties and device performance.

The objective of this work was to develop a computationally efficient approach for studying defect-containing perovskites at larger length and time scales than are practical with conventional first-principles molecular dynamics alone.

I developed and evaluated **machine-learned interatomic potentials (MLIPs)** using the MACE message-passing neural network. The models were trained on ab initio molecular dynamics (AIMD) data and used to perform molecular dynamics simulations of FAPbBr₃ systems containing different types of point defects.

---

## My Contributions

I worked across the computational workflow, from generating and preparing AIMD training data to training machine-learning models, evaluating model performance, running molecular dynamics simulations, and analyzing the resulting structural and electronic properties.

### AIMD Data Generation

I generated and analyzed **_ab initio_ molecular dynamics (AIMD)** data for FAPbBr₃ systems with different structural configurations and defect types.

The systems included defect-free bulk crystals as well as systems containing vacancy, interstitial, Frenkel, and Schottky defects. I also investigated different system sizes and temperatures to provide training data spanning a range of structural configurations.

The AIMD calculations used density-functional-theory-based methods and provided the energies, forces, and atomic configurations needed to train the machine-learning potentials.

### Machine Learned Interatomic Potentials

I trained **MACE machine-learning models** to reproduce the energetic and force behavior obtained from AIMD simulations.

I investigated how the composition of the training dataset affected model performance by training multiple models using different combinations of defect-free and defect-containing systems. I evaluated model accuracy using metrics including energy RMSE, force RMSE, and relative force error.

The best-performing model achieved substantially lower errors than the other models, demonstrating the importance of selecting appropriate training data for accurately representing the underlying potential energy surface.

### Iterative Model Development

I developed an iterative computational workflow for improving the machine-learning potentials.

The workflow involved running AIMD simulations, training MACE models, performing MACE molecular dynamics simulations, evaluating model stability and accuracy, and continuing model training to reduce prediction error.

This approach allowed me to systematically evaluate model performance and determine how additional or different training data affected the ability of the MLIP to reproduce ab initio behavior.

### Molecular Dynamics & Structural Analysis

I used the trained MACE potentials to perform molecular dynamics simulations of larger FAPbBr₃ systems.

I analyzed the resulting trajectories to investigate structural behavior using techniques including mean-square displacement (MSD) and radial distribution function (RDF) analysis. These calculations provided information about atomic motion, structural stability, and local coordination within the perovskite crystal.

### Electronic Structure Analysis

I investigated how defects influence the electronic properties of FAPbBr₃ by analyzing **band structures and density of states**.

I performed electronic-structure calculations for bulk and larger FAPbBr₃ systems and examined the resulting band structures and projected density of states (PDOS) to identify changes associated with different structural configurations.

---

## Tools & Skills

**Computational Chemistry & Machine Learning**

- Molecular dynamics
- Density functional theory
- electronic structure calculations
- machine learned interatomic potentials
- MACE
- CP2K

**Programming & Data Analysis**

- Python
- Data analysis
- Scientific visualization

**Computational Environment**

- Linux
- High-performance computing
- Command-line workflows
- Python notebooks

---

## Results

I trained and evaluated multiple MACE models using different combinations of AIMD data.

The models showed substantial differences in predictive accuracy depending on the systems included in their training datasets. The strongest model achieved training errors of 0.3 meV/atom for energy and 8.6 meV/Å for forces, with validation errors of 0.3 meV/atom and 12.5 meV/Å, respectively.

The trained MLIPs were then used to perform molecular dynamics simulations and investigate structural behavior through MSD and RDF analyses. The resulting simulations provided a computationally efficient way to examine defect-containing FAPbBr₃ systems.

I also investigated the electronic consequences of structural and defect changes through band structure and density-of-states calculations, providing insight into how defects can alter the electronic properties of FAPbBr₃.

---

## Deliverables

### Presentation

[View the project presentation (PDF)](https://rxchel.github.io/rachellee/assets/files/perovskite-defects/presentation.pdf)

---

## Project Takeaways

This project gave me experience with the end-to-end workflow of a machine-learning-driven computational materials research project:

AIMD simulations → data generation → MLIP training → model evaluation → molecular dynamics → structural analysis → electronic structure calculations → scientific communication

Through this work, I developed practical experience with machine learning, molecular dynamics, density functional theory, computational materials science, defect modeling, scientific programming, and quantitative model evaluation.

More broadly, the project demonstrated how machine learning can bridge the gap between accurate but computationally expensive _ab initio_ methods and large-scale simulations needed to understand complex materials behavior.
