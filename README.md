# Heart Disease Classification

## Overview

This project implements an end-to-end supervised machine learning workflow for predicting the presence of heart disease using the UCI Heart Disease Dataset.

The project focuses on data preprocessing, model training, comparison of multiple classification algorithms, model interpretation, and evaluation of the trade-off between predictive performance and interpretability.

## Objectives

- Understand and preprocess the heart disease dataset
- Identify and handle missing values and duplicate records
- Encode categorical variables appropriately
- Apply feature scaling where required
- Train and evaluate multiple supervised learning models
- Tune and interpret a Decision Tree classifier
- Extract human-readable rules from a Decision Tree
- Experiment with k-Nearest Neighbors (kNN)
- Compare ensemble learning methods
- Evaluate models using accuracy, F1-score, and ROC-AUC
- Discuss model interpretability, risks, and limitations

## Machine Learning Workflow

### 1. Data Preprocessing

The preprocessing workflow includes:

- Missing-value handling
- Duplicate checking
- Removal of irrelevant columns
- Target binarization
- One-hot encoding of categorical variables
- Feature scaling using standardization
- Stratified train-test splitting

### 2. Baseline Models

The following baseline classifiers were evaluated:

- Logistic Regression
- Naive Bayes

### 3. Decision Tree

A Decision Tree classifier was trained and tuned using:

- `max_depth`
- `min_samples_split`
- `min_samples_leaf`

Feature importance and decision paths were also examined.

### 4. Rule-Based Classification

A shallow Decision Tree was used to extract human-readable IF-THEN rules and examine the trade-off between interpretability and predictive performance.

### 5. k-Nearest Neighbors

kNN was evaluated using multiple values of `k`:

- 1
- 3
- 5
- 7
- 9

Different distance metrics were also explored.

### 6. Ensemble Learning

Ensemble methods included:

- Random Forest
- Gradient Boosting
- AdaBoost

These models were compared with the baseline and individual classifiers.

## Results

The experiments showed that **Random Forest achieved the strongest overall predictive performance** among the evaluated models.

The final analysis reported:

- Accuracy: **0.8641**
- F1-score: **0.8631**
- ROC-AUC: **0.9207**

The Rule-Based model provided the most interpretable predictions through simple IF-THEN rules.

## Key Insights

The analysis identified several important predictors of heart disease, including:

- Asymptomatic chest pain
- Maximum heart rate achieved
- ST depression

The project also highlights an important machine learning trade-off: models with stronger predictive performance can be less interpretable, while simpler rule-based models are easier for users to understand.

## Repository Contents

| File | Description |
|---|---|
| `heart_disease_classification.ipynb` | Complete machine learning analysis and modelling notebook |
| `heart_disease_classification_report.pdf` | Assignment report |
| `README.md` | Project documentation |

## Tools & Technologies

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Dataset

The project uses the **UCI Heart Disease Dataset**.

The dataset contains patient medical records and the classification task predicts whether a patient has heart disease or not.

## Model Interpretation & Limitations

The project considers practical risks associated with deploying machine learning models in healthcare, including false negatives, dataset bias, model explainability, and model staleness.

The results should therefore be interpreted as an academic machine learning exercise rather than a clinical diagnostic system.

## Academic Project

This project was completed as part of a Machine Learning course assignment covering supervised learning, preprocessing, model comparison, decision trees, rule-based classification, kNN, and ensemble learning.
