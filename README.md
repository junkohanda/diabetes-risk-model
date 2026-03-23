# diabetes-risk-model
# Project Summary

This machine learning project develops a predictive model for diabetes risk using approximately 97,000 healthcare records sourced from Kaggle. The analysis excludes gestational and Type 1 diabetes cases and implements safeguards against data leakage to maintain clinical rigor.

**Research Focus:**
This project examines how differences in training data distribution — particularly the demographic composition of the dataset — may affect model generalizability across populations. The goal is to understand the model's behavior and limitations, not to attribute performance differences to biological or racial characteristics.

**Technical Implementation:**
Logistic regression was implemented using scikit-learn, achieving a ROC-AUC score of 0.934 and an accuracy of 0.89. Features include age, ethnicity, BMI, sleep duration, exercise frequency, HbA1c levels, and insulin measurements.

**Development Stack:**
Python, pandas, scikit-learn, matplotlib, seaborn, Google Colab

**Next Steps:**
Planned work includes evaluating performance across varied data distributions, comparing results with gradient boosting models such as LightGBM, and conducting fairness assessments across demographic segments.

---

> **Disclaimer:** This project is developed for educational and learning purposes only. The model and its outputs are not intended for clinical use, medical diagnosis, or any healthcare decision-making. Do not use this tool as a substitute for professional medical advice.




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
