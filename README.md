# AI-Assisted-Analysis
AI-assisted data analysis and visualization supporting experimental research.

# AI-Assisted Analysis

This repository contains AI-assisted data analysis, optimization, machine-learning modeling, and model-interpretation workflows developed to support experimental research.

The repository is organized into four main research sections:

- Hydrometallurgy
- Briquette
- Bituminous Mastic
- Mortar (Cement)

## Hydrometallurgy

The Hydrometallurgy section contains data analysis and visualization of elemental concentrations in leachate samples.

The analysis includes:

- EN 888 compliance classification
- Quality scoring
- Hierarchical clustering
- Comparison of Cr, Ni, and Mn concentrations

[View Hydrometallurgy analysis](./Hydrometallurgy/)

## Briquette

The Briquette section contains AI-assisted analysis of briquette performance.

The analysis includes:

- Compression strength
- Durability
- Standardized hierarchical clustering
- Numerical linkage analysis
- Performance comparison among briquette formulations

[View Briquette analysis](./Briquette/)

## Bituminous Mastic

The Bituminous Mastic section contains modeling and interpretation of the Aging Index of bituminous mastics.

The evaluated methods include:

- Genetic Algorithm (GA)
- Particle Swarm Optimization (PSO)
- Artificial Neural Network (ANN)
- Gaussian Process Regression (GPR)
- Support Vector Regression (SVR)
- SHAP model interpretation

A shared experimental dataset is used across the different modeling approaches.

[View Bituminous Mastic analysis](./Bituminous_Mastic/)

## Mortar (Cement)

The Mortar section contains two main analysis categories:

### Mechanical Properties

The mechanical-property analysis focuses on:

- Maximum flexural stress
- Mean compressive strength

The evaluated methods include:

- GA and PSO empirical-model optimization
- ANN
- GPR
- SVR
- SHAP interpretation

### Gauge Factor

The Gauge Factor analysis focuses on predicting the average final gauge factor (GFend).

The workflow includes:

- PCHIP interpolation
- Akima interpolation
- ANN
- GPR
- SVR
- Nested Leave-One-Out Cross-Validation
- SHAP interpretation

[View Mortar (Cement) analysis](./Mortar(Cement)/)

## Repository Structure

```text
AI-Assisted-Analysis/
├── README.md
├── Hydrometallurgy/
├── Briquette/
├── Bituminous_Mastic/
└── Mortar(Cement)/
```

## Reproducibility

The notebooks document the data preparation, statistical analysis, optimization, machine-learning modeling, validation, visualization, and model-interpretation procedures used in the corresponding research sections.

Each analysis folder contains its associated notebooks and documentation to support reproducibility of the reported results.
