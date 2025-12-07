# Explaining-Wages-with-Econometric-Models
Econometric analysis of how gender, education, and experience explain variation in hourly wages, using a cross-sectional dataset of 1,472 individuals.

🚀 Overview

This project uses the BWAGES dataset to estimate wage determinants using OLS, dummy variables, interaction effects, and heteroskedasticity-robust inference.

The analysis proceeds in three stages:
- Part A: Baseline OLS with education dummies and experience
- Part B: Interaction between gender and education
- Part C: White standard errors, residual diagnostics, and distributional tests

🛠️ Methods

Part A – Baseline Wage Model
- Descriptive statistics
- Creation of education dummies (educ1–educ5)
- OLS model:
  wage = β0 + β1 male + β2 educ1 + ... + β5 exper + ε
- Interpretation of coefficients & significance
- Predicted wage for a male university graduate
- Extension: add exper² to capture nonlinear returns to experience

Part B – Gender × Education Interaction
- Build a model allowing wage differences across gender within each education level
- OLS estimation with interaction terms
- Test gender differences jointly
- Show that:
  SSR_pooled(model with interactions) = SSR_men + SSR_women
  (two-sample decomposition)

Part C – Robustness & Diagnostics
- Compute White (heteroskedasticity-robust) standard errors
- Compare with classical OLS SEs
- Residual diagnostics:
  - Residual distribution plot
  - Correlation between residuals & experience
  - Normality test (e.g., Shapiro–Wilk, KS, Jarque–Bera)
- Discussion of implications if normality is rejected (e.g., t-tests validity, inference robustness)
