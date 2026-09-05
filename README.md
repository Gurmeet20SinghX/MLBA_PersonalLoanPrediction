# Job Market Analytics: Salary Prediction & Location Preference Modelling

A capstone analytics project using machine learning and statistical analysis to study salary determinants and Delhi/NCR location preference in the Indian job market.

> **Academic project:** Capstone II — Analytics, Great Lakes Institute of Management  
> **Team project:** Gurmeet Singh and team

## Executive Overview

The project addresses two related business problems:

1. **Salary Prediction (Regression):** estimate candidate salary using experience, education, skills, location and functional area.
2. **Location Preference (Classification):** predict whether a candidate prefers Delhi/NCR to support targeted talent acquisition and workforce-planning decisions.

The final analysis works from a large job-seeker dataset and applies a reproducible data-quality pipeline, exploratory analysis, NLP-based feature engineering, statistical validation, supervised learning, class-imbalance handling and external validation.

## Data & Processing

- Initial records: **907,675**
- Valid records after cleaning/outlier controls: **559,332**
- Modelling sample: **50,000** using stratified random sampling
- Raw variables: **17**
- Engineered features: **121+**, including TF-IDF skill features and NLP-derived seniority
- Key controls included age/experience validation, salary cleaning, missing-value treatment, city standardisation and target-leakage prevention.

## Analytics Approach

### Exploratory & Statistical Analysis

- Univariate and bivariate analysis
- Salary distribution and experience analysis
- Education and geographic salary comparisons
- Functional-area analysis
- Delhi/NCR preference analysis
- Chi-square tests for categorical associations
- Correlation analysis

### Feature Engineering

- Salary cleaning and log transformation
- Work-experience parsing and categorisation
- Education standardisation
- City standardisation
- NLP seniority extraction
- **TF-IDF** vectorisation of skills
- Leakage prevention by excluding variables derived from the target

### Machine Learning

**Regression:** Linear/Ridge/ElasticNet/Huber and tree/boosting approaches were evaluated, with model selection focused on generalisation rather than training performance.

**Classification:** Logistic Regression, Decision Tree, Random Forest and Gradient Boosting approaches were evaluated, including **SMOTE** for class imbalance.

## Key Findings

- Work experience was the strongest salary predictor, with correlation **r = 0.399**.
- Delhi/NCR showed an estimated **15–20% salary premium** over several tier-2 locations in the analysed sample.
- Education was materially associated with salary; the analysis estimated approximately **20–30% premium for Master's** and **40–50% for PhD** versus Bachelor's in the sample.
- **75.96%** of the modelling sample indicated Delhi/NCR preference, creating a substantial class-imbalance challenge.
- Current city and functional area were among the strongest predictors of location preference.
- External validation exposed meaningful population/data shift, reinforcing the importance of testing model generalisation outside the training distribution.

## Model Performance Highlights

### Salary Regression

The final model selection prioritised robust generalisation. The conservative Gradient Boosting approach achieved approximately **R² = 0.235** on the held-out test set, with **RMSE ≈ 0.579**. The report notes that the lower performance reflects distribution differences and limited explanatory variables rather than simply a failure of model complexity.

### Location Preference Classification

Random Forest with SMOTE produced the strongest held-out F1 among the compared models at approximately **0.697**, while Gradient Boosting achieved approximately **73.8% test accuracy**. The final external test validation also showed that population shift can materially change apparent model performance.

## Business Applications

The analysis translates model outputs into practical use cases for:

- **Recruitment:** data-driven salary ranges and candidate targeting
- **HR analytics:** salary benchmarking, pay-band analysis and workforce planning
- **Talent acquisition:** location-preference targeting and relocation strategy
- **Career analytics:** scenario-based salary and location decisions

## Limitations & Responsible Interpretation

The project explicitly identifies data-distribution mismatch as a major limitation. The external test set had a very different Delhi/NCR preference distribution from the modelling sample, demonstrating why strong training performance should not automatically be treated as real-world performance.

Predictions should therefore be interpreted as **sample-specific analytical outputs**, not universal salary or relocation guarantees.

## Repository Structure

```text
.
├── README.md
├── requirements.txt
└── capstone/
    ├── README.md
    ├── MODELING_NOTES.md
    ├── DATA_AND_REPRODUCIBILITY.md
    └── report/
        └── README.md
```

## Skills Demonstrated

**Python · Pandas · NumPy · Scikit-learn · Statistical Testing · EDA · NLP · TF-IDF · Feature Engineering · Regression · Classification · SMOTE · Cross-Validation · Model Evaluation · Data Quality · Business Analytics · Data-driven Recommendations**

## Academic Source

Final report: *Job Market Analytics: Salary Prediction and Location Preference Modelling*, Capstone II — Analytics. The report identifies Gurmeet Singh as a member of Group 1. 
