# Hospital Readmission Prediction After Thyroidectomy

## Overview
This project develops a machine learning model to predict hospital readmissions following thyroidectomy surgery. Early prediction of potential readmissions can help healthcare providers take preventive measures and improve patient outcomes.

## Problem Statement
Hospital readmissions after thyroidectomy represent both a patient care concern and a healthcare cost issue. This model aims to identify patients at high risk of readmission using pre-operative and immediate post-operative data.

## Methods
- **Data Processing**: Cleaned and preprocessed clinical data, handling missing values and outliers
- **Feature Engineering**: Created new features from existing clinical parameters
- **Model**: Implemented XGBoost, Catboost and LightGBM
- **Evaluation**: Used metrics including AUC ROC, balanced accuracy, precision, recall, and F1-score

## Key Findings
- Readmission rate was <1%, making classification challenging
- Among the tested models, LightGBM performed the best (LGBM > Catboost > Xgboost)
- The best model achieved and AUROC of 91% on this highly imbalanced dataset
- Top factors contributing to readmission risk were:
  1. TSH/FT4 ratio
  2. PACU PTH
  3. Calcium/PTH Ratio
  4. BMI

Interestingly, a few features that were created such as TSH/FT4 ratio and Calcium/PTH ratio contributed significantly to the prediction of readmission, **possibly indicating their use in clinical settings** for risk analysis.
