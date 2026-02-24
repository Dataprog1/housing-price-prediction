# Housing Price Prediction

Machine learning project for housing price prediction using feature engineering and model optimization.

This project was developed as part of a Machine Learning lab, based on the  
Sberbank Russian Housing Market Kaggle competition.

The goal was to build a model that predicts apartment prices based on property characteristics and macro-related information.

---

## Project Overview

Rather than relying on a simple regression model, the project explores how different modeling approaches and feature engineering techniques improve prediction accuracy.

The project is divided into three main parts:

### Part 1 — Regression

- Built a Random Forest regression model
- Evaluated performance using:
  - Random 80/20 split
  - Time-based split (train on earlier data → test on later data)
- Compared results to understand how time affects prediction quality

---

### Part 2 — Classification

Focused on a specific sub-area:

- Calculated price per square meter
- Divided apartments into 4 percentile-based price levels
- Built a Random Forest classifier to predict price category
- Evaluated performance using:
  - Confusion Matrix
  - Precision & Recall

---

### Part 3 — Model Improvements

Starting from the baseline model, several improvements were introduced:

- Feature importance analysis
- Handling missing values based on skewness
- Binning construction year into categories
- Fixing data inconsistencies (e.g. unrealistic build years)
- Using macro-related adjustments
- Moving to an XGBoost model
- Selecting top 20 most important features

Final performance:

- Cross-validation score: ~0.67 R²

---

## Models Used

- Decision Tree
- Random Forest
- XGBoost

---

## Techniques Applied

- Feature Engineering
- Label Encoding
- Time-based validation
- K-Fold Cross Validation
- Handling skewed distributions
- Feature Importance selection

---

## Key Insight

The project highlights how:

Accounting for time effects and improving feature handling can significantly impact housing price predictions.

Simple models provide a baseline — but meaningful improvements come from data understanding and iterative refinement.

---

## Project Files

- 📒 Notebook:  
  `notebooks/housing_price_model.ipynb`

- 📄 Project Summary:  
  `results/project_summary.pdf`
