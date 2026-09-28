# Mortar (Cement) – AI-Assisted Analysis

This folder contains the AI-assisted analyses developed for cement mortar mixtures.

Two main research directions are investigated:

- Mechanical Properties
- Gauge Factor (GF)

---

## Mechanical Properties

The mechanical property analysis focuses on predicting:

- Maximum flexural stress
- Mean compressive strength

The input variables are:

- Sludge content
- Plasticizer dosage
- Density

The following modelling approaches are evaluated:

- Genetic Algorithm (GA)
- Particle Swarm Optimization (PSO)
- Artificial Neural Network (ANN)
- Gaussian Process Regression (GPR)
- Support Vector Regression (SVR)

Model interpretation is performed using SHAP analysis based on the GPR models.

The complete analysis is available in:

`Mechanical_Properties/`

---

## Gauge Factor (GF)

The Gauge Factor analysis investigates the prediction of the average final gauge factor (GFend) of mortar mixtures.

The input variables are:

- Sludge content
- Plasticizer dosage

Due to the limited number of experimental conditions, interpolation methods are applied:

- PCHIP interpolation
- Akima interpolation

The interpolated datasets are used for predictive modelling using:

- Artificial Neural Network (ANN)
- Gaussian Process Regression (GPR)
- Support Vector Regression (SVR)

SHAP analysis is applied for interpretation of the selected GPR model.

The complete analysis is available in:

`Gauge_Factor/`

---

## Repository Structure

