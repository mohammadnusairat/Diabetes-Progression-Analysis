# Diabetes Progression Analysis

**Course**: STAT 481 — Applied Statistical Methods  
**Student**: Mohammad Nusairat  
**Date**: April 1, 2025

---

## 📌 Project Overview

This project investigates the progression of diabetes using a dataset of 442 patients, originally introduced in the paper *Least Angle Regression* by Efron et al. Our primary goal is to identify which clinical and biochemical baseline features most strongly predict a patient's disease progression after one year.

We perform thorough exploratory data analysis, correlation inspection, diagnostic checking, and multiple linear regression to construct and evaluate predictive models. 

---

## 📊 Dataset Description

The dataset includes 10 numerical baseline predictors and 1 response variable:

- **AGE**: Patient’s age
- **SEX**: Binary gender (1 = Male, 2 = Female)
- **BMI**: Body mass index
- **BP**: Average blood pressure
- **S1–S6**: Various blood serum measurements  
  - S1: Total cholesterol  
  - S2: LDL  
  - S3: HDL  
  - S4: Cholesterol/HDL ratio  
  - S5: Triglyceride level  
  - S6: Blood sugar level
- **Target**: Diabetes progression after one year (response variable)

---

## 🧪 Statistical Techniques Used

### 🔍 Exploratory Data Analysis (EDA)
- Five-number summaries (min, Q1, median, Q3, max)
- Mean, standard deviation, and distributional properties
- Boxplots and histograms for visual analysis
- Correlation matrix and heatmap to examine multicollinearity

### 📈 Modeling Approaches
- **Multiple Linear Regression (MLR)**  
  Used to assess the overall fit and significance of each variable.
  
- **Model Selection Techniques**:
  - **Adjusted R²** and **Mallows’ Cp** for choosing optimal models
  - **Stepwise selection** for feature reduction
  - **Variance Inflation Factor (VIF)** to detect multicollinearity

- **Residual Diagnostics**:
  - Residual vs Fitted plots
  - Normal Q-Q plots
  - Scale-Location plots
  - Residual leverage and Cook’s distance

- **Transformation & Refinement**:
  - Evaluating normality of residuals
  - Addressing skewness or outliers
  - Comparing full vs reduced models

---

## 🧰 Technologies Used

- **R** (via RStudio)
- **R Markdown** for reproducible reporting
- Core packages: `ggplot2`, `car`, `MASS`, `dplyr`, `corrplot`, `olsrr`

---

## 📁 Project Files

- `Diabetes.txt`: Dataset used for analysis  
- `Diabetes Progression Analysis.Rmd`: R Markdown source file  
- `Diabetes-Progression-Analysis.pdf`: Final report  
- `Diabetes-Progression-Analysis_HTML.html`: Rendered HTML output  
- `LeastAngle_2002.pdf`: Reference paper describing the original dataset  
- `README.md`: This documentation

---

## ✅ Outcomes

- BMI, BP, S5 (triglycerides), and S6 (blood sugar) showed the strongest predictive power for disease progression.
- S1 and S2 were highly correlated, potentially leading to multicollinearity.
- A reduced linear model was developed using statistically significant predictors, balancing simplicity and predictive strength.

---

## 📌 References

- Efron, B., Hastie, T., Johnstone, I., & Tibshirani, R. (2004). *Least Angle Regression*. Annals of Statistics.
- Hastie, T., Tibshirani, R., & Friedman, J. (2009). *The Elements of Statistical Learning*.
