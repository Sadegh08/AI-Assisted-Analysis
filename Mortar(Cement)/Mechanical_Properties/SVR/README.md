# SVR Analysis of Mortar Mechanical Properties

This folder contains the Support Vector Regression (SVR) analysis developed for predicting the mechanical properties of cement mortar mixtures.

## Analysis

The SVR models use the following input variables:

- Sludge content
- Plasticizer dosage
- Density

Two mechanical responses are predicted:

- Maximum flexural stress
- Mean compressive strength

## SVR Model

Support Vector Regression models are developed using different kernel functions:

- Radial Basis Function (RBF)
- Polynomial
- Linear
- Sigmoid

Hyperparameters are optimized using grid-search cross-validation.

## Validation

Model performance is evaluated using Leave-One-Out Cross-Validation (LOOCV).

In each iteration, one observation is held out as the test sample, while the remaining observations are used for model training and parameter selection.

## Model Performance

Prediction performance is evaluated separately for flexural strength and compressive strength using:

- R²
- RMSE
- MAE
- MAPE

## Input Data

The analysis uses the experimental dataset containing:

- Sludge content
- Plasticizer dosage
- Density
- Maximum flexural stress
- Mean compressive strength

## Notebook

The complete SVR analysis is available in:

`SVR.ipynb`

## Outputs

The notebook generates:

- Kernel comparison results
- Optimized SVR parameters
- LOOCV predictions
- Flexural strength performance metrics
- Compressive strength performance metrics
- Measured-versus-predicted plots
- Numerical result export

## Reproducibility

The SVR workflow applies the same dataset and validation framework for both mechanical response variables.

Leave-One-Out Cross-Validation is used to evaluate model performance and generalization.
