# ANN Analysis of Mortar Mechanical Properties

This folder contains the Artificial Neural Network (ANN) analysis developed for predicting the mechanical properties of cement mortar mixtures.

## Analysis

The ANN model uses the following input variables:

- Sludge content
- Plasticizer dosage
- Density

The model predicts two target variables simultaneously:

- Maximum flexural stress
- Mean compressive strength

## ANN Model

A multi-output Artificial Neural Network is used to predict both mechanical responses within a single modelling framework.

The input and output variables are standardized before model training.

## Validation

Model performance is evaluated using Leave-One-Out Cross-Validation (LOOCV).

In each iteration, one specimen is held out for testing and the model is trained using the remaining observations.

Hyperparameter selection is performed using grid-search cross-validation.

## Model Performance

Prediction performance is evaluated separately for flexural strength and compressive strength using:

- R²
- RMSE
- MAE
- MAPE

## Input Data

The analysis uses the unified experimental dataset containing:

- Sludge content
- Plasticizer dosage
- Density
- Maximum flexural stress
- Mean compressive strength

## Notebook

The complete ANN analysis is available in:

`ANN.ipynb`

## Outputs

The notebook generates:

- LOOCV predictions
- Flexural-strength performance metrics
- Compressive-strength performance metrics
- Selected ANN hyperparameters
- Measured-versus-predicted plots
- Final trained ANN model
- Numerical result export

## Reproducibility

The ANN workflow uses Leave-One-Out Cross-Validation and standardized input and output variables.

The same dataset and modelling framework are used for both mechanical response variables.
