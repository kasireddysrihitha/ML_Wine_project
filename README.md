# 🍷 Wine Quality Prediction Using Ridge, Lasso and Elastic Net Regression

## 📌 Project Overview

This project focuses on predicting the numerical quality score of red wine samples using physicochemical properties of the wine.

The project compares three regularized linear regression techniques:

- Ridge Regression
- Lasso Regression
- Elastic Net Regression

The objective is to study how regularization techniques perform when predicting wine quality from correlated physicochemical features.

---

## 🎯 Problem Statement

Wine quality is influenced by several measurable physicochemical properties such as acidity, sulphates, alcohol content, density, and sulfur dioxide levels.

This project formulates wine quality prediction as a supervised regression problem, where the numerical `quality` score is predicted from 11 physicochemical measurements.

---

## 📊 Dataset

**Dataset:** WineQT.csv

- Rows: 1,143
- Columns: 13
- Target variable: `quality`
- Predictor variables: 11 physicochemical features
- Identifier: `Id`

The `Id` column is excluded from model training because it is only an identifier and has no chemical meaning.

### Input Features

- Fixed Acidity
- Volatile Acidity
- Citric Acid
- Residual Sugar
- Chlorides
- Free Sulfur Dioxide
- Total Sulfur Dioxide
- Density
- pH
- Sulphates
- Alcohol

### Target

`quality`

The quality scores in this dataset range from 3 to 8.

---

## 🔍 Exploratory Data Analysis

The EDA includes:

- Dataset structure and basic statistics
- Missing-value analysis
- Duplicate-value analysis
- Target distribution
- Feature distributions
- Outlier analysis
- Feature-target correlations
- Correlation matrix
- Multicollinearity analysis

Some notable relationships observed during EDA include a positive association between alcohol and quality and a negative association between volatile acidity and quality.

---

## ⚙️ Methodology

The project follows this workflow:

```text
Wine Quality Dataset
        ↓
Data Inspection & Cleaning
        ↓
Exploratory Data Analysis
        ↓
Feature / Target Separation
        ↓
Remove Id
        ↓
80/20 Train-Test Split
        ↓
StandardScaler
        ↓
Ridge / Lasso / Elastic Net
        ↓
5-Fold Cross-Validation
        ↓
Prediction
        ↓
Model Evaluation
        ↓
Model Comparison
