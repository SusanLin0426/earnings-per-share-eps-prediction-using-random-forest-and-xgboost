# EPS Prediction with Random Forest and XGBoost

This repository contains the final project for the course **Applications of Machine Learning and Data Analysis in Accounting**.

The project applies **Random Forest** and **XGBoost** models to predict EPS (Earnings Per Share) of Taiwanese listed companies using financial statement data (balance sheet, income statement, cash flow statement). The results are further applied to **portfolio construction and investment evaluation**.

---

## Contents
- `B08303006_final.ipynb`: Google Colab Jupyter Notebook containing the implementation.  
- `B08303006_final.pdf`: Written project report, including methodology, results, and investment implications.  

---

## Project Overview

### Data Processing
- EPS adjustment for comparability.  
- Normalization of financial statement accounts (scaled by total assets or operating revenue).  
- Handling missing values (imputation or removal).  

### Models
- Random Forest (with Grid Search for hyperparameter tuning).  
- XGBoost (Gradient Boosting framework).  
- Evaluation metrics: **RMSE** (Root Mean Squared Error) and **MAE** (Mean Absolute Error).  

### Analysis
- Prediction of EPS for **all industries (2017)**.  
- Prediction of EPS for the **semiconductor industry (2017)**.  
- Comparison of model accuracy and variable importance.  
- Portfolio construction using **EPS growth (ΔEPS) signals**.  

---

## Key Findings
- **XGBoost** generally outperforms Random Forest in prediction accuracy.  
- Important predictors include:  
  - Adjusted EPS (t-1, t-2)  
  - Retained earnings & undistributed profits  
  - Long-term debt (corporate bonds payable)  
  - Net income attributable to parent company  
  - Capital surplus  

---

## Visuals
The notebook includes:  
- EPS prediction vs. actual (line charts).  
- RMSE/MAE comparison plots.  
- Variable importance rankings for both Random Forest and XGBoost.  
- Portfolio allocation pie charts and performance tables.  

---

## Requirements
The code was run on **Google Colab** with the following Python libraries:  

```bash
pandas
numpy
scikit-learn
xgboost
matplotlib
seaborn
