# Capstone II — Job Market Analytics

## Salary Prediction and Location Preference Modelling

### Project purpose

This capstone analyses the Indian job market using predictive analytics to address two business questions:

- Can candidate salary be estimated from experience, education, skills, location and functional area?
- Can Delhi/NCR location preference be predicted to support targeted talent acquisition and workforce-planning decisions?

### Dataset and pipeline

The final report describes an initial dataset of **907,675 job-seeker records**. After city, age, salary and experience quality controls, **559,332 valid records** remained and a stratified sample of **50,000** was used for modelling. The feature set expanded from 17 raw variables to more than 120 engineered features, including TF-IDF skill features and NLP-derived seniority.

### Analytical workflow

1. Data quality assessment and cleaning
2. Exploratory data analysis
3. Salary and experience analysis
4. Education, city and functional-area analysis
5. Delhi/NCR location-preference analysis
6. Statistical validation using correlation and chi-square tests
7. Feature engineering and NLP/TF-IDF processing
8. Regression and classification model development
9. Cross-validation and model comparison
10. External test-set validation
11. Business interpretation and recommendations

The modelling work uses Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, SciPy and TF-IDF-based text processing.

### Key analytical findings

- Work experience was the strongest numeric predictor of salary (**r = 0.399**).
- Delhi/NCR preference represented **75.96%** of the modelling sample, creating a substantial class-imbalance problem.
- Current city and functional area showed strong associations with location preference.
- Higher education was associated with higher salary in the analysed sample.

### Modelling & validation

The project evaluates multiple regression and classification approaches and uses cross-validation to compare generalisation. For classification, SMOTE was used to address the 3:1 class imbalance. The final report also documents external validation, where the test population had a materially different NCR-preference distribution; this was treated as a data-shift/generalisation issue rather than hidden or ignored.

### Important result

The final report identifies **Gradient Boosting** as the strongest conservative regression approach, with approximately **R² = 0.235** on the held-out test set. For location classification, **Random Forest with SMOTE** produced the strongest held-out F1 among the compared models at approximately **0.697**.

### Business value

The project translates technical analysis into business applications for:

- salary benchmarking and compensation analytics;
- targeted recruitment and talent acquisition;
- workforce planning and location strategy;
- career and relocation decision support.

### Academic project

**Capstone II — Analytics**  
Great Lakes Institute of Management  
Group 1 — Gurmeet Singh and team
