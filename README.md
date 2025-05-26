
# ORCA DFT-Based Machine Learning Force Field for Water Molecules

This project aims to develop a high-accuracy, machine learning-based force field for water clusters using **Density Functional Theory (DFT)** calculations performed with **ORCA**. The trained model will replicate quantum-level interactions and be evaluated by comparing its predictions with **experimental data** and **standard force fields** such as **TIP3P** and **SPC/E**.

>  Project Status: Actively in Progress – Files, data, and training results will be uploaded progressively.

---

##  Objectives

- Perform DFT calculations on water clusters using ORCA 
- Extract forces, energies, and optimized geometries from ORCA outputs 
- Train a machine learning potential using frameworks like **NequIP** 
- Compare predicted physical and thermodynamic properties with:
  - Experimental reference data
  - Classical force fields (TIP3P, SPC/E)

---

##  Tools

| Tool       | Role                                  |
|------------|---------------------------------------|
| **ORCA**   | DFT calculations (energies, forces, geometries) |
| **ASE**    | Molecular modeling & job automation   |
| **Python** | Data parsing, conversion, and scripting |
| **NequIP** | E(3)-equivariant neural network training |
| **Ovito**  | Molecular structure visualization     |

---

##  Workflow

```mermaid
graph TD
    A[Build Water Clusters] --> B[Run ORCA DFT Calculations]
    B --> C[Extract Forces, Energies, and Coordinates]
    C --> D[Train Neural Network (e.g., NequIP)]
    D --> E[Predict Molecular Behavior]
    E --> F[Compare with Experimental & TIP3P/SPC/E Results]
```

---

## Folder Structure (Plan)

```bash
orca-dft-ml-forcefield-water/
├── orca_dft/            # Input/output files for ORCA
├── data_extraction/     # Python scripts for parsing ORCA results
├── training_data/       # Cleaned data for ML model input
├── nequip_training/     # Training scripts, config files, logs
├── analysis/            # Evaluation scripts and plots
├── results/             # Benchmark results and comparisons
├── README.md
└── requirements.txt     # Required packages and dependencies
```

---

## Properties for Evaluation

The ML force field will be evaluated against experimental data and TIP3P/SPC/E models for:

- Radial Distribution Functions (RDF)
- Bond length and angle distributions
- Dipole moment


---

## Author
Handson Gisubizo 
MSE ChemBE @ Johns Hopkins University 
GitHub: [handsongisubizo](https://github.com/handsongisubizo) 
Email: hgisubi1@jh.edu

---
