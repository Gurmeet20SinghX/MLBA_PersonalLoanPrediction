# MLBA_PersonalLoanPrediction
Predicting personal loan acceptance using logistic regression and decision tree models with SMOTE and hyperparameter tuning. Includes data cleaning, EDA, model evaluation, and business-focused insights to guide decisions. MLBA End Term Group Project with detailed workflow and results.

# Personal Loan Prediction (MLBA End Term Project)

This repository contains our MLBA end-term group project focused on predicting personal loan acceptance using machine learning models.

## 📊 Project Overview

- **Objective:** Predict personal loan acceptance based on customer demographic, financial, and product ownership features.
- **Models Used:**
  - Logistic Regression (with and without SMOTE)
  - Decision Tree (with SMOTE & hyperparameter tuning)
- **Tools:** Python, Pandas, Scikit-learn, Matplotlib, Seaborn

## 📁 Repository Structure

- `notebooks/`: Project notebook with complete workflow.
- `reports/`: Final group report for submission.
- `results/`: Visualizations of evaluation metrics and feature importance.
- `src/`: Modular reusable Python scripts for preprocessing, model training, and evaluation.
- `data/`: Contains the dataset (add if permitted by your institution).

📈 Results Summary
Logistic Regression Accuracy: ~94%

Logistic Regression + SMOTE Recall: Increased from 45% to 91%

Decision Tree Accuracy: ~96% with higher recall and F1-score

AUC: ~0.96 indicating strong classification ability
