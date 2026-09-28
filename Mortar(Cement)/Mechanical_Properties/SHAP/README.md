# SHAP Analysis of Mortar Mechanical Properties

This folder contains the SHAP (SHapley Additive exPlanations) analysis developed for interpreting the Gaussian Process Regression (GPR) models used for predicting the mechanical properties of cement mortar mixtures.

## Analysis

SHAP is applied to explain the contribution of input variables to the predictions of GPR models.

The interpreted input variables are:

- Sludge content
- Plasticizer dosage
- Density

The analysed target responses are:

- Maximum flexural stress
- Mean compressive strength

## SHAP Method

Kernel SHAP is used to calculate feature contributions for the GPR predictions.

Separate SHAP analyses are performed for:

- Flexural strength prediction
- Compressive strength prediction

## Model Interpretation

The SHAP analysis provides:

- Feature contribution values
- Global feature importance based on mean absolute SHAP values
- Summary plots showing the effect of input variables on model predictions

The SHAP results describe the behaviour of the trained GPR models and do not represent direct causal relationships.

## Input Data

The analysis uses the experimental dataset containing:

- Sludge content
- Plasticizer dosage
- Density
- Maximum flexural stress
- Mean compressive strength

## Notebook

The complete SHAP analysis is available in:

`SHAP_GPR.ipynb`

## Outputs

The notebook generates:

- SHAP values for flexural strength
- SHAP values for compressive strength
- Feature importance analysis
- SHAP summary plots
- Numerical SHAP result export

## Reproducibility

The SHAP workflow uses the trained GPR models developed for the mechanical property prediction task.

The same input variables and dataset are used for interpretation of both mechanical responses.
