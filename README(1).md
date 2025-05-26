# ORCA DFT-Based Machine Learning Force Field for Water Molecules

This project develops a high-accuracy machine learning force field for water clusters using Density Functional Theory (DFT) calculations from ORCA. The trained model replicates quantum-level interactions and will be validated against experimental data and classical force fields such as TIP3P and SPC/E.

> Project Status: In Progress — Files, data, and training results will be uploaded progressively.

---

## Objectives

- Perform DFT calculations on water clusters using ORCA 
- Extract energies, forces, and optimized geometries from ORCA outputs 
- Train a neural network potential (e.g., NequIP)  
- Evaluate model predictions by comparing with:
  - Experimental reference data 
  - Classical force fields (TIP3P, SPC/E)

---

## Tools

| Tool       | Purpose                                        |
|------------|------------------------------------------------|
| ORCA       | DFT calculations (energies, forces, geometries)|
| ASE        | Molecular modeling and job automation          |
| Python     | Parsing, conversion, and scripting             |
| NequIP     | E(3)-equivariant neural network training       |
| Ovito      | Structure visualization                        |

---

## Workflow

```mermaid
graph TD
    A[Build Water Clusters] --> B[Run ORCA DFT Calculations]
    B --> C[Extract Forces, Energies, and Coordinates]
    C --> D[Train Neural Network (e.g., NequIP)]
    D --> E[Predict Molecular Behavior]
    E --> F[Compare with Experimental & TIP3P/SPC/E Results]
```

---

## Folder Structure (Planned)

```
orca-dft-ml-forcefield-water/
├── orca_dft/            # ORCA input/output files
├── data_extraction/     # Scripts to parse ORCA outputs
├── training_data/       # Cleaned data for ML input
├── nequip_training/     # Training scripts, configs, logs
├── analysis/            # Evaluation scripts and plots
├── results/             # Benchmark results and comparisons
├── README.md
└── requirements.txt     # Dependencies
```

---

## Properties for Evaluation

The trained machine learning force field will be evaluated against experimental data and classical models (TIP3P, SPC/E) using:

- Bond length and angle distributions  
- Radial Distribution Functions (RDF)  
- Dipole moments  
- Energy and force consistency with DFT results

---

## Author

**Handson Gisubizo**  
MSE Chemical & Biomolecular Engineering  
Johns Hopkins University  
 Email: [hgisubi1@jh.edu](mailto:hgisubi1@jh.edu)  
 GitHub: [handsongisubizo](https://github.com/handsongisubizo)
