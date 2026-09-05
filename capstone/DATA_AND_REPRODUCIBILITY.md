# Data & Reproducibility

## Data scope

The capstone report states that the source data contained 907,675 job-seeker records from 2021. After quality controls, 559,332 valid records remained and a stratified sample of 50,000 records was used for modelling.

The final modelling pipeline applies age and experience controls, salary cleaning, missing-value treatment, city standardisation and feature engineering. The feature set expands from 17 raw variables to more than 120 engineered features.

## Reproducibility controls

- Fixed random state: 42
- Stratified random sampling for the modelling sample
- Saved feature structure and preprocessing parameters
- Reused fitted encoders/vectorisers for external test processing
- Five-fold cross-validation for model comparison
- Separate external test validation

## Data leakage control

Preferred-location fields are excluded from the feature matrix because the classification target is derived from the preferred-location information. This prevents circular reasoning.

## Data availability

Only non-sensitive, appropriate-to-share project materials should be committed to a public repository. Do not upload confidential employer/customer information or any dataset whose redistribution is not permitted.
