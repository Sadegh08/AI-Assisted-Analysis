# Mortar (Cement) – AI-Assisted Analysis

This folder contains the AI-assisted analyses developed for cement mortar mixtures.

Two main analysis categories are investigated:

- Mechanical Properties
- Gauge Factor (GF)

## Mechanical Properties

The mechanical property analysis focuses on predicting:

- Maximum flexural stress
- Mean compressive strength

The input variables are:

- Sludge content
- Plasticizer dosage
- Density

The evaluated methods include:

- Genetic Algorithm (GA)
- Particle Swarm Optimization (PSO)
- Artificial Neural Network (ANN)
- Gaussian Process Regression (GPR)
- Support Vector Regression (SVR)

GA and PSO are used to optimize the coefficients of empirical models for the mechanical responses.

ANN, GPR, and SVR are used as machine-learning regression models.

SHAP analysis is used to interpret the GPR model predictions.

The analyses are available in:

- [GA_PSO](./Mechanical_Properties/GA_PSO/)
- [ANN](./Mechanical_Properties/ANN/)
- [GPR](./Mechanical_Properties/GPR/)
- [SVR](./Mechanical_Properties/SVR/)
- [SHAP](./Mechanical_Properties/SHAP/)

## Gauge Factor (GF)

The Gauge Factor analysis focuses on predicting the average final gauge factor (GFend) of cement mortar mixtures.

The input variables are:

- Sludge content
- Plasticizer dosage

Because of the limited number of experimental mixture conditions, two interpolation methods are applied:

- Piecewise Cubic Hermite Interpolating Polynomial (PCHIP)
- Akima interpolation

The interpolated datasets are evaluated using:

- Artificial Neural Network (ANN)
- Gaussian Process Regression (GPR)
- Support Vector Regression (SVR)

Model performance is evaluated using Nested Leave-One-Out Cross-Validation (LOOCV).

SHAP analysis is applied to interpret the selected GPR model.

The complete Gauge Factor analysis is available in:

- [Gauge_Factor](./Gauge_Factor/)

## Repository Structure

```text
Mortar(cement)/
├── README.md
│
├── Mechanical_Properties/
│   ├── GA_PSO/
│   │   ├── README.md
│   │   └── GA_and_PSO.ipynb
│   ├── ANN/
│   │   ├── README.md
│   │   └── ANN.ipynb
│   ├── GPR/
│   │   ├── README.md
│   │   └── GPR.ipynb
│   ├── SVR/
│   │   ├── README.md
│   │   └── SVR.ipynb
│   └── SHAP/
│       ├── README.md
│       └── SHAP_GPR.ipynb
│
└── Gauge_Factor/
    ├── README.md
    └── Mortar_GFend_Modeling.ipynb
```

## Reproducibility

The notebooks document the data preparation, model development, validation, prediction, and interpretation procedures used in the analyses.

The corresponding modelling and validation frameworks are applied consistently within each analysis to support reproducibility of the reported results.
