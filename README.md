# Personal Loan Acceptance Prediction

A machine learning project focused on predicting whether a customer is likely to accept a personal loan offer. The project combines exploratory data analysis, feature preparation, class-imbalance handling, supervised classification, model evaluation, and business interpretation.

## Project Objective

Banks and financial institutions can use customer-level data to identify prospects who are more likely to accept relevant loan offers. The objective of this project is to build and compare classification models that predict personal-loan acceptance and translate model findings into practical business insights.

## Business Problem

The project addresses a common banking analytics problem:

> **Given a customer's demographic, financial, and product-ownership information, can we predict whether the customer will accept a personal loan offer?**

A reliable prediction model can help improve customer targeting, reduce unnecessary outreach, and support more data-driven campaign decisions.

## Dataset

The project uses a bank customer dataset containing demographic, financial, and banking-product attributes. The target variable represents personal-loan acceptance.

The dataset is included in the repository as `bankloan.xlsx`.

## Approach

1. **Data preparation** – inspect the dataset, handle data-quality issues, and prepare variables for modelling.
2. **Exploratory Data Analysis (EDA)** – analyse customer characteristics and relationships with loan acceptance.
3. **Feature preparation** – select and transform relevant predictors for classification.
4. **Class-imbalance treatment** – apply **SMOTE (Synthetic Minority Over-sampling Technique)** to improve the model's ability to identify the minority class.
5. **Model development** – build and compare:
   - Logistic Regression
   - Logistic Regression with SMOTE
   - Decision Tree with SMOTE
   - Decision Tree with hyperparameter tuning
6. **Model evaluation** – assess accuracy, recall, precision, F1-score, ROC-AUC, confusion matrix, and precision-recall performance.
7. **Business interpretation** – translate model outputs into insights relevant to customer targeting and loan marketing decisions.

## Key Results

The analysis reported the following approximate outcomes:

| Model / Approach | Result |
|---|---|
| Logistic Regression | ~94% accuracy |
| Logistic Regression + SMOTE | Recall improved from ~45% to ~91% |
| Decision Tree | ~96% accuracy with strong recall/F1 performance |
| ROC-AUC | ~0.96 |

The results demonstrate the importance of evaluating more than accuracy when the business objective includes identifying customers who are likely to accept the loan offer. SMOTE materially improved minority-class recall in the analysis.

## Technologies & Libraries

- Python
- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn
- Matplotlib
- Seaborn
- Jupyter Notebook
- Excel (`.xlsx`)

## Repository Contents

```text
.
├── MLBA Project Code.ipynb   # End-to-end analysis and modelling workflow
├── bankloan.xlsx             # Project dataset
├── README.md                 # Project documentation
├── requirements.txt          # Python dependencies
└── .gitignore                # Files excluded from version control
```

## How to Run

1. Clone or download the repository.
2. Install the required Python packages:

```bash
pip install -r requirements.txt
```

3. Open `MLBA Project Code.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
4. Run the notebook from top to bottom to reproduce the analysis.

## Portfolio Highlights

This project demonstrates practical skills in:

- Exploratory Data Analysis
- Data Cleaning & Feature Preparation
- Classification Modelling
- Imbalanced Classification using SMOTE
- Model Comparison
- Hyperparameter Tuning
- Model Evaluation
- Data Visualization
- Business-focused Interpretation

## Academic Project

**MLBA End-Term Group Project**

Developed as part of the Data Science & Analytics curriculum at Great Lakes Institute of Management.
