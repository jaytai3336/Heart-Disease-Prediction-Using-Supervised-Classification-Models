# 🫀 Heart Disease Prediction - DSA1101 Individual Assignment

This repository contains the completed individual assignment for **DSA1101: Data Science in Practice**. The task was to analyze a heart disease dataset and determine the most suitable classification model to predict whether a patient is likely to have heart disease based on a variety of medical attributes.

## 📌 Project Objective

- Explore and preprocess a heart disease dataset (300 patients, 13 attributes).
- Identify significant predictors of heart disease.
- Train and evaluate multiple classification models.
- Determine the best-performing classifier based on relevant evaluation metrics.

## 📊 Dataset Overview

The dataset includes both **quantitative** and **categorical** variables related to patient health. The response variable is `<disease>` (presence or absence of heart disease). Examples of features include:
- `age`, `bp`, `chol`, `heart.rate`, `vessels` (Quantitative)
- `sex`, `chest.pain`, `fbs`, `resting.ecg`, `angina`, `blood.disorder` (Categorical)

Missing values in `<blood.disorder>` were imputed using the mode.

## 🧪 Models Applied

Four supervised classifiers were implemented and compared using **5-fold cross-validation**:
- 🌳 **Decision Tree**
- 🧮 **Naïve Bayes**
- 📈 **Logistic Regression**
- 📍 **K-Nearest Neighbors (KNN)**

## 📈 Evaluation Metrics

Each model was evaluated using:
- **True Positive Rate (TPR)**: Critical due to medical context (false negatives are high risk)
- **Precision**
- **Receiver Operating Characteristic (ROC) Curve**
- **Area Under the Curve (AUC)**

## ✅ Results Summary

| Classifier        | TPR   | Precision | AUC   |
|-------------------|-------|-----------|--------|
| Decision Tree     | 0.797 | 0.859     | 0.893 |
| Naïve Bayes       | 0.804 | 0.841     | 0.912 |
| Logistic Regression | 0.928 | 0.621     | 0.872 |
| **K-Nearest Neighbors** | **0.826** | **0.905** | **0.953** |

➡️ **KNN** was selected as the best model due to its high TPR, precision, and AUC.

## ⚖️ Tradeoffs and Considerations

- KNN is sensitive to feature scaling and irrelevant variables.
- It performs well for small to moderate-sized datasets but may not scale efficiently.
- Unlike Logistic Regression, it doesn’t provide clear interpretability of predictor importance.

## 📁 File Structure

📄 DSA1101 Individual Assignment.docx   # Final report with analysis and visualizations

⚠️ Note: The original `.Rmd` file was unfortunately corrupted and could not be uploaded.

📝 This README was generated with assistance from ChatGPT.

