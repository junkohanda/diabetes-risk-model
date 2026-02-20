# diabetes-risk-model

## Overview
This project builds a machine learning model to predict diabetes risk using a large-scale healthcare dataset (~97,000 samples) from Kaggle.

The project incorporates clinical insights from nursing practice, including:
- Exclusion of gestational diabetes and Type 1 diabetes
- Prevention of data leakage
- Clinically meaningful feature selection

In addition to model performance, this study explores a key research question:

> Can a model trained primarily on Asian population data generalize to other ethnic groups?

---

## Dataset
- Source: Kaggle Healthcare Dataset
- Sample size: ~97,000
- Features include:
  - Age
  - Ethnicity
  - BMI
  - Sleep time
  - Exercise time
  - HbA1c
  - insulin level

---

## Model
- Logistic Regression (scikit-learn)

---

## Performance
- ROC-AUC: **0.934**
- Accuracy: **0.89**

The model demonstrates strong discriminative performance while maintaining interpretability.

---

## Tools & Technologies
- Python
- pandas
- scikit-learn
- matplotlib
- seaborn
- Google Colab

---

## Future Work
- External validation on multi-ethnic datasets
- Comparison with gradient boosting models (e.g., LightGBM)
- Fairness evaluation across demographic groups
