# Virtual Screening and ML Model for Anti-Cancer Compounds Targeting MetAP2

This repository contains the work for a two-phase project focused on identifying potential anti-cancer compounds from turmeric that target Methionine Aminopeptidase 2 (MetAP2) in liver cancer patients.

## Authors
- Hanna (@slack)
- BigWils (@slack)
- Samar_samir (@slack)
- Sarasamer22 (@slack)
- DerleenM (@slack)

## Project Overview

### Phase 1: Virtual Screening by Molecular Docking
In this phase, we conducted virtual screening of turmeric phytochemicals against MetAP2 using molecular docking techniques.

Key steps:
1. Curated a library of 51 turmeric phytochemicals
2. Prepared the MetAP2 protein structure (PDB ID: 1R58)
3. Performed molecular docking using PyRx
4. Analyzed binding affinities and visualized top compounds using PyMOL

### Phase 2: Machine Learning Model for IC50 Prediction
We developed a machine learning model to predict the IC50 (half maximal inhibitory concentration) of compounds against MetAP2.

Key components:
- Dataset: ChEMBL database (version 34)
- Molecular descriptors: Generated using RDKit and Mordred
- Model: Random Forest Regressor
- Evaluation metrics: MSE, MAE, R-squared

## Repository Structure

```
├── Binding_site_parameters/
├── Docking_Result/
├── Ligands + binding affinities + predicted pIC50/
├── ML project python script/
├── Phase_one_report/
├── Phase_two_report/
├── Phytochemicals_SDF_structures/
├── Phytochemicals_libareries/
├── Prepared_protein_PDB_structure/
└── README.md
```

## Key Findings

1. Top binding compounds from docking:
   - Cyclocurcumin
   - Curcumol
   - Tetrahydrocurcumin
   - Demethoxycurcumin

2. ML model performance:
   - MSE: 0.0504
   - MAE: 0.0952
   - R-squared: 0.9647

3. Positive correlation observed between binding affinity and predicted pIC50 values

## Getting Started
1. Navigate to the `ML project python script/` directory for the machine learning model
2. Refer to `Phase_one_report/` and `Phase_two_report/` for detailed methodologies and results

## Results Visualization

The `Docking_Result/` directory contains visualizations of the top compounds docked with MetAP2. The `Ligands + binding affinities + predicted pIC50/` folder provides comprehensive data on the ligands, their binding affinities, and predicted pIC50 values.

## Data Sources

- Phytochemical structures and libraries are available in the `Phytochemicals_SDF_structures/` and `Phytochemicals_libareries/` directories
- The prepared protein structure can be found in `Prepared_protein_PDB_structure/`

## Acknowledgments

We thank the HackBio [https://course.thehackbio.com/] for providing this learning opportunity.

