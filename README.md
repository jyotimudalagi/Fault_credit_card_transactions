# Fault_credit_card_transactions
A machine learning workflow to detect credit card fraud in highly imbalanced datasets. Includes EDA, feature scaling, and comparative modeling using Logistic Regression and Random Forest, evaluated with ROC-AUC and Precision-Recall (PR-AUC) metrics to effectively identify fraudulent transactions.

## Objective
Identify **fraudulent credit card transactions** using machine learning.

## Dataset Overview
The dataset contains anonymized credit card transactions labeled as fraud or not.

- `Time`, `Amount`, and anonymized features `V1` to `V28`
- `Class`: 1 for fraud, 0 for non-fraud

## Workflow
1. Load and explore the dataset
2. Handle class imbalance
3. Feature scaling and model training
4. Evaluate performance

## Exploratory Data Analysis

## Data Preprocessing

## Model Training

## Evaluation

## Conclusion
- Built and compared two models — Logistic Regression and Random Forest — for binary fraud classification.
- Addressed feature scaling (`Amount`, `Time`) and class imbalance using `class_weight='balanced'`.
- Evaluated using confusion matrix, precision/recall/F1, ROC-AUC, and Precision-Recall AUC (more meaningful than plain accuracy given the ~0.17% fraud rate).
- Random Forest's feature importances highlight which anonymized `V` features contribute most to detecting fraud.
- Future work: try ensemble methods (e.g. XGBoost, LightGBM), SMOTE/undersampling for resampling, threshold tuning to balance precision vs recall, and cross-validation for more robust performance estimates.
