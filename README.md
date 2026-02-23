# MD Analysis and MM/PBSA Toolkit

A reproducible post-processing workflow for Molecular Dynamics (MD) simulations performed with GROMACS, integrating structural stability analysis and MM/PBSA binding free energy evaluation.

This repository provides a unified Jupyter notebook implementing publication-ready analysis and automated energy parsing for protein–ligand systems.

---

## Overview

The workflow supports:

- Structural stability assessment
- Interaction persistence evaluation
- Secondary structure monitoring
- Global MM/PBSA binding energy analysis
- Per-residue energy decomposition with automated residue selection

All figures are generated in publication-ready format (vector + high-resolution raster).

---

## Implemented Analyses

### Structural Analysis
- Root-Mean-Square Deviation (RMSD)
- Root-Mean-Square Fluctuation (RMSF)
- Radius of Gyration (Rg)
- Solvent Accessible Surface Area (SASA)
- Hydrogen Bond Analysis (including occupancy %)
- DSSP-based secondary structure evolution

### Energetic Analysis (MM/PBSA)
- Global energy term parsing
- Wide-format energy table generation
- Binding energy comparison plots
- Per-residue energy decomposition
- Automated identification of stabilising/destabilising residues

---

## Computational Assumptions

- MD Engine: GROMACS (2021+ compatible)
- Trajectory format: `.xtc`
- Topology format: `.tpr`
- MM/PBSA output: `g_mmpbsa` summary files
- Energy units: kJ/mol (GROMACS convention)

The workflow is compatible with GPU-accelerated and HPC-based simulations.

---

## Repository Structure
