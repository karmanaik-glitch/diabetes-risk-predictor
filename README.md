# Diabetes Risk Predictor

## Overview
A machine learning model to screen patients for diabetes risk 
using clinical measurements. Built as part of a Healthcare AI/ML 
learning journey.

## Dataset
Pima Indians Diabetes Database — 768 patients, 8 clinical features

## Models Compared
- Logistic Regression — AUC: 0.84
- Decision Tree — AUC: 0.76  
- Random Forest — AUC: 0.83
- SVM — AUC: 0.81

## Best Model
Logistic Regression / Tuned Random Forest (AUC = 0.84, CV = 0.84 ± 0.02)

## Key Findings
- Glucose, BMI and Age are the strongest predictors
- Threshold tuned to 0.4 to improve recall for diabetic patients
- Clinical reasoning: recall prioritised over precision for screening use case
- Cross validation revealed Decision Tree overfits despite decent single-split AUC

## Tools Used
Python · Pandas · Scikit-learn · Matplotlib · Seaborn · Google Colab

## Clinical Context
Model acts as a screening tool — not a diagnostic confirmation. 
High recall prioritised to minimise missed diabetic patients.
