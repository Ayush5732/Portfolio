# Housing Price Regression Analysis (Ames Dataset)

## Overview
This project applies rigorous regression analysis techniques to the Ames Housing dataset to model residential property values. Rather than focusing solely on raw predictive metrics, the primary objective is to build a **statistically valid multiple linear regression model** by systematically evaluating core assumptions and implementing advanced remedial measures for violations.

## Objectives
* Build a robust multiple linear regression model to predict and interpret housing prices.
* Systematically evaluate classical linear regression model (CLRM) assumptions.
* Diagnose and apply formal remedial measures for assumption violations (e.g., heteroskedasticity, non-normality).
* Maximize both the interpretability of coefficients and predictive performance.

## 📊 Dataset
* **Source:** Ames Housing Dataset (Available on [[Kaggle](https://www.kaggle.com/))](https://www.kaggle.com/datasets/shashanknecrothapa/ames-housing-dataset)
* **Description:** Contains detailed residential property records from Ames, Iowa, featuring high-dimensional data points across structural quality, space, location, and transactional metrics.

## Methodology

### 1. Data Preparation & Preprocessing
* Handled missing data structures and encoded categorical variables.
* Multi-collinearity diagnosis using Variance Inflation Factors (VIF) to refine feature selection.

### 2. Baseline Modeling & Diagnostics
* Fitted an initial Multiple Linear Regression (OLS) model.
* Conducted residual diagnostics via Q-Q plots, Residual vs. Fitted plots, and formal statistical testing.

### 3. Assumption Testing & Issues Identified
* **Non-Normality:** Residuals exhibited right-skewness, failing the Shapiro-Wilk test.
* **Heteroskedasticity:** Non-constant variance detected across the predicted spectrum (confirmed via Breusch-Pagan test).

### 4. Remedial Measures & Advanced Modeling
* **Log-Transformation:** Applied a natural log transformation to the response variable (`SalePrice`) to stabilize variance and normalize errors.
* **Generalized Least Squares (GLS):** Employed a GLS approach (via the `nlme` package) to model the error structure directly and correct for non-constant variance.

## Results & Impact
* **Assumption Alignment:** Log transformations and GLS corrections successfully mitigated heteroskedasticity and restored residual normality.
* **Model Fidelity:** Improved model fit
* **Reliability:** Standard errors were successfully corrected, ensuring that coefficient p-values are valid for reliable real-world statistical inference.

## Tools & Technologies
* **Language:** R
* **Core Packages:** `tidyverse` (dplyr, ggplot2), `car` (VIF & companion diagnostics), `nlme` (GLS modeling), `lmtest`

## 🧠 Key Takeaways
* **Production-Ready Rigor:** Prioritized statistical validity and strict CLRM assumption testing over blind hyperparameter tuning, ensuring the model's insights are reproducible and reliable.
* **Feature Engineering & Transformations:** Utilized log-transformations and structural modeling modifications (GLS) to elegantly fix structural errors in messy, real-world data patterns.
* **Balanced Evaluation:** Proved that optimizing for inference and coefficient integrity is just as critical as chasing raw predictive performance.

## 🚀 Future Improvements
* **Regularization:** Implement Ridge and Lasso regression to handle high-dimensional feature spaces and prevent overfitting.
* **Non-Linear Extensions:** Explore generalized additive models (GAMs) to capture non-linear trends smoothly.
* **Machine Learning Benchmark:** Compare the inferential model against tree-based ensemble methods (e.g., XGBoost, Random Forests) to evaluate prediction trade-offs.

---
**Author:** Ayush Chaudhary  
*Graduate Student, Data Analytics*
