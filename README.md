# 🏦 Term Deposit Subscription Prediction Using Machine Learning

This repository contains a supervised learning project focused on predicting whether clients of a Portuguese bank will subscribe to term deposit products. The project applies classification models, sampling techniques, and feature engineering strategies to address real-world marketing challenges in the banking industry.

---

## 📌 Project Overview

- **Objective**: Forecast client subscription decisions to optimize marketing strategy and resource allocation.
- **Dataset Source**: [UCI Machine Learning Repository – Bank Marketing Dataset](https://archive.ics.uci.edu/dataset/222/bank+marketing)
- **Data Format**: `bank_additional-full.csv`, 41,188 records, 21 features.

---

## 🔍 Problem Statement

The goal is to classify whether a client will subscribe (`yes`) or not (`no`) to a term deposit using demographic, economic, and campaign-related features. Key challenges include:
- Severe class imbalance
- High-dimensional categorical features
- Feature correlation and redundancy

---

## 📊 Models Implemented

- Gaussian Naïve Bayes
- Logistic Regression
- Random Forest Classifier
- Support Vector Machine (SVM)
- Neural Network (Keras with TensorFlow backend)

Each model was tested with:
- No Sampling
- Random Oversampling
- Random Undersampling
- SMOTE (Synthetic Minority Oversampling Technique)

---

## ⚙️ Feature Engineering

- Age binning to create age groups
- Transformation of `pdays` to binary (previous contact vs. none)
- Composite economic indicator from highly correlated features
- One-Hot and Label Encoding for categorical features

---

## 📈 Evaluation Metrics

- Accuracy
- Precision & Recall
- F1-Score
- ROC-AUC Score

Models were benchmarked using stratified K-Fold cross-validation to ensure balanced performance assessment.

---

## ✅ Key Insights

- **Logistic Regression (No Sampling)**: Best precision for classifying non-subscribers (91%)
- **SVM (Undersampling)**: Best recall for identifying potential subscribers (67%)
- **Random Forest**: High interpretability and balanced performance
- **Neural Network**: Promising results with early stopping to prevent overfitting

---

## 💡 Strategic Impact

- Improved targeting of likely subscribers → higher conversion rates.
- Resource optimization by avoiding outreach to uninterested clients.
- Identified misclassified but high-potential leads for retargeting.
