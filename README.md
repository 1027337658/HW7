## Overview
This repository contains a complete solution to the Week 8 Bayesian Homework assignment. The homework is divided into three main questions:

1. **Q1: Analytical Derivations for Linear Regression**  
   - Derivation of the posterior distribution for the regression coefficients \(\boldsymbol \beta\) given a Gaussian likelihood and a multivariate Normal prior.
   - Derivation of the posterior distribution for the error variance \(\sigma^2\) using an Inverse-Gamma prior.
   - (Optional Extra) Demonstration of the connection between the log-posterior under Normal/Laplace priors and the ridge/lasso loss functions.

2. **Q2: Bayesian Linear Regression**  
   - Implementation of a Bayesian linear regression model on an interesting dataset.
   - The model uses independent `pm.Normal` priors for the regression coefficients and a half–Normal prior for \(\sigma\) (instead of an inverse–gamma prior).
   - Full posterior inference is provided along with MCMC diagnostics and posterior predictive checks.

3. **Q3: Robust Bayesian Linear Regression**  
   - Implementation of a robust Bayesian linear regression model that accounts for heavy-tailed errors by introducing observation-specific latent variables \(\tau_i\).
   - The model is applied to data with outliers, and the posterior distributions of \(\tau_i\) are used to identify potential outlier observations.
   - An influence analysis based on the hat matrix for weighted least squares is performed to compare the influence of outlier versus non-outlier observations.
   - MCMC diagnostics and full Bayesian posterior analysis are provided.

## Requirements
- numpy
- scipy
- matplotlib
- pymc
- arviz
- plotly

## File Structure
- **hw8.ipynb**: The main Jupyter Notebook containing the full solution. It is organized into clearly delineated sections for Q1, Q2, and Q3, with written explanations in markdown cells and executable code cells that generate all required plots and diagnostic images.
- **CarPrice_Assignment.csv**：The Data uesd from https://www.kaggle.com/code/zabihullah18/car-price-prediction?select=CarPrice_Assignment.csv.
