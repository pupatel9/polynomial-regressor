# polynomial-regressor

## Overview

This project provides a comprehensive, from-scratch implementation and in-depth analysis of **1D polynomial regression**, focusing on generating synthetic datasets, implementing and comparing several loss functions, fitting polynomial models via numerical optimization, and performing detailed model evaluation using residual plots, bootstrap bias-variance estimation, and model comparison.

All functionality is implemented using only base `numpy`, `matplotlib`, and `scipy`, ensuring transparency and educational value. The code is designed for clarity and extensibility, making it ideal for foundational statistical experiments.

---

## Features

- **Synthetic Data Generation and Visualization**
  - Generate 1D polynomial datasets with adjustable noise and degree.
  - Visualize noisy samples and the true underlying function.

- **Loss Function Implementations**
  - Includes MSE, MAE, Hinge Loss, Log Loss (Binary Cross-Entropy), and LINEX Loss.
  - All loss functions implemented manually using NumPy for maximum transparency.

- **Model Fitting with Custom Loss Functions**
  - Fit polynomials of arbitrary degree using `scipy.optimize.minimize`.
  - Use any of the supported loss functions for training.

- **Residual Analysis and Diagnostics**
  - Plot test residuals and compare fitted models to ground truth on unseen data.
  - Includes train-test splitting and consistent performance evaluation.

- **Bootstrap Bias-Variance Estimation**
  - Generate multiple bootstrap samples with out-of-bag (OOB) tracking.
  - Visualize per-sample bias and variance for different model complexities.

- **Model Comparison and Evaluation**
  - Compare underfit, well-fit, and overfit models using bootstrap statistics.
  - Structured estimator wrapper class simplifies training/prediction routines.

---

## Notable Design Choices
- **No Black-box Libraries:**
  - All regressors, losses, and visualizations were built directly from fundamental numerical operations, without using scikit-learn or similar high-level APIs.

- **Well-Commented Code:**
  - Every function includes comprehensive docstrings for clarity.
 
- **Modular Structure:**
  - All algorithms and utilities are reusable as standalone functions or classes.
    
## Project Applications
  - Ideal for understanding the theory behind regression and model assessment.
  - Demonstrates hands-on mastery of the bias-variance tradeoff, custom loss optimization, and residual analysis.
