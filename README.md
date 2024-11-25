# Anti_Doping_Model

This repository contains a machine learning pipeline for predicting athlete sanctions based on biological, test, and sport-related data. The model uses a *Random Forest Classifier* with SMOTE for handling imbalanced data and cross-validation to evaluate its performance.

## Features

- *Preprocessing*: 
  - Numerical features are standardized using StandardScaler.
  - Categorical features are encoded using OneHotEncoder.

- *Model*: 
  - Random Forest Classifier with class balancing to handle imbalanced target classes.
  - SMOTE (Synthetic Minority Oversampling Technique) is used to address class imbalance in the training data.

- *Evaluation*:
  - Accuracy, precision, recall, and F1 scores are reported.
  - Cross-validation to validate model robustness.

## Dataset

The dataset includes the following features:

- Sport: The sport category of the athlete.
- Doping Suspicion Score: A numerical score indicating suspicion of doping.
- Supplements Used: Types of supplements used by the athlete.
- Hemoglobin, Reticulocytes, Urea, Creatinine: Biological data.
- Biological Passport Data: Information related to the athlete's biological passport.
- Test Result: Outcome of doping tests.

The target variable is Sanctioned, which indicates whether the athlete is sanctioned (Yes or No).

## Requirements

Install the required libraries using the following command:

```bash
pip install pandas scikit-learn imbalanced-learn numpy
