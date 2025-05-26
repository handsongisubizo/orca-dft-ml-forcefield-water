# ORCA DFT-Based Machine Learning Force Field for Water Molecules

This project develops a high-accuracy machine learning force field for water clusters using Density Functional Theory (DFT) calculations from ORCA. The trained model will replicate quantum-level interactions and be validated against experimental data and classical models such as TIP3P and SPC/E.

> Project Status: In Progress — Files, data, and training results will be uploaded progressively.

---

## Objectives

- Perform DFT calculations on water clusters using ORCA  
- Extract energies, forces, and optimized geometries from ORCA outputs  
- Train a neural network potential (e.g., NequIP)  
- Evaluate model predictions by comparing with:
  - Experimental data  
  - Classical force fields (TIP3P, SPC/E)

---

## Tools

| Tool       | Purpose                                        |
|------------|------------------------------------------------|
| ORCA       | DFT calculations (energies, forces, geometries)|
| ASE        | Molecular modeling and job automation          |
| Python     | Parsing, conversion, scripting                 |
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
    
    

## Properties for Evaluation

The ML force field will be evaluated against experimental data and TIP3P/SPC/E models for:
- Bond length and angle distributions
- Others 



## Author
Handson Gisubizo 
MSE ChemBE @ Johns Hopkins University 
GitHub: [handsongisubizo](https://github.com/handsongisubizo) 
Email: hgisubi1@jh.edu


