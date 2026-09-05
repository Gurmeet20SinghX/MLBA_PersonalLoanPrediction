# Modelling Notes

## Targets

- Regression target: `Salary_Cleaned` / log-transformed salary
- Classification target: `Prefers_Delhi_NCR`

## Regression

The project compares regularised linear and tree/boosting approaches. The final report prioritises generalisation because the dataset shows distribution mismatch between training and external data. The conservative Gradient Boosting model achieved approximately R² = 0.235 on the held-out test set.

## Classification

The location-preference target is imbalanced, with approximately 75.96% of the modelling sample preferring Delhi/NCR. SMOTE is applied to the training data to improve minority-class detection. Random Forest with SMOTE achieved the strongest held-out F1 among the compared models at approximately 0.697.

## Validation

Five-fold cross-validation is used during model comparison. External validation is also performed using a separate test population. The external test set shows a major change in NCR-preference prevalence, so external performance must be interpreted in the context of population/data shift.

## Leakage control

The implementation explicitly excludes variables derived from the target, including preferred-location fields used to construct the Delhi/NCR preference target. This avoids circular prediction.

## Feature engineering

The project includes salary and experience cleaning, city and education standardisation, seniority extraction from titles, TF-IDF skill features, target transformations and categorical encoding.
