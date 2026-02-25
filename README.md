# MD Analysis and MM/PBSA Toolkit

A reproducible post-processing workflow for Molecular Dynamics (MD) simulations performed with GROMACS. The notebook integrates structural stability analysis and MM/PBSA binding free energy evaluation for protein–ligand systems.

---

## Scope

The workflow includes:

- RMSD (global structural stability)
- RMSF (residue flexibility)
- Radius of Gyration (compactness)
- SASA (solvent exposure)
- Hydrogen bond analysis (with occupancy)
- DSSP secondary structure analysis
- Global MM/PBSA energy parsing
- Per-residue energy decomposition with automated hotspot selection

All figures are exported in publication-ready formats (PDF, SVG, high-resolution PNG).

---

## Computational Assumptions

- Engine: GROMACS (2021+)
- Trajectory: `.xtc`
- Topology: `.tpr`
- MM/PBSA output: `g_mmpbsa`
- Energy units: kJ/mol (native GROMACS convention)

Compatible with GPU-accelerated and HPC-based simulations.

---

## Installation

pip install -r requirements.txt

---

## Usage

jupyter notebook md_analysis_and_mmpbsa_workflow.ipynb

Update file paths to your local MD and MM/PBSA outputs and execute all cells sequentially.

---

## Reproducibility

- Native energy units preserved
- Automatic ps → ns time conversion
- Deterministic parsing and residue selection
- Vector-format figure export

---

MIT License.
