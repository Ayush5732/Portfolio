# Housing Price Regression Analysis (Ames Dataset)

## Overview

This project applies regression analysis techniques to the Ames Housing dataset to understand the relationship between housing features and sale price. The goal is to build a statistically valid model while carefully evaluating assumptions and applying corrective measures where needed.

---

## 📊 Objectives

* Build a multiple linear regression model for housing prices
* Evaluate model assumptions (normality, homoscedasticity, etc.)
* Apply remedial measures when assumptions are violated
* Improve model performance and interpretability

---

## 🗂️ Dataset

* Ames Housing Dataset
* Contains detailed residential property data such as size, location, quality, and sale price

---

## ⚙️ Methodology

### 1. Data Preparation

* Data cleaning and preprocessing
* Handling missing values
* Feature selection

### 2. Initial Model

* Multiple linear regression model
* Evaluation using R² and residual diagnostics

### 3. Assumption Testing

* Normality of residuals
* Homoscedasticity (constant variance)
* Linearity
* Independence

### 4. Issues Identified

* Non-normal residual distribution
* Presence of heteroscedasticity

### 5. Remedial Measures

* Log transformation of response variable
* Generalized Least Squares (GLS) approach
* Model re-evaluation after corrections

---

## 📈 Results

* Improved model fit after transformations
* Better adherence to regression assumptions
* More reliable coefficient estimates

---

## 🛠️ Tools & Technologies

* R
* Libraries: (e.g., ggplot2, dplyr, nlme, car)

---

## 📁 Project Structure

* `code/` → R scripts for analysis
* `report/` → Final report (no code)

---

## 🚀 Key Takeaways

* Checking assumptions is critical in regression modeling
* Transformations can significantly improve model validity
* Statistical rigor is as important as predictive performance

---

## 🔮 Future Improvements

* Try non-linear models
* Use regularization techniques (Lasso/Ridge)
* Compare with machine learning models

---

## 👤 Author

[Your Name]
