# Heart Failure Survival Prediction

## Project Overview
This project explores clinical records to predict the occurrence of death events among patients with heart failure. It uses exploratory data analysis, machine learning classification models, cross-validation, and hyperparameter tuning.

## Dataset
The dataset is the Heart Failure Clinical Records dataset from the UCI Machine Learning Repository.

Dataset source: https://archive.ics.uci.edu/dataset/519/heart+failure+clinical+records

It contains 299 patient records with clinical and demographic features. The target variable, `DEATH_EVENT`, indicates whether a death event occurred during the follow-up period.

## Models
The project compares:
- Logistic Regression
- Linear Discriminant Analysis (LDA)
- Quadratic Discriminant Analysis (QDA)

Logistic Regression and QDA are also tuned using cross-validation.

## Evaluation
Models are evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion matrices and ROC curves

The dataset is divided into training and testing sets using a stratified 80:20 split. Five-fold stratified cross-validation is used for model comparison and tuning.

## Repository Structure
- `data/` — Original and cleaned datasets
- `notebooks/01_cleaning_eda.ipynb` — Data cleaning and exploratory analysis
- `notebooks/02_models.ipynb` — Baseline classification models
- `notebooks/03_validation_tuning.ipynb` — Cross-validation and hyperparameter tuning
- `report/` — Model evaluation results in CSV format

## Results Summary
In the baseline test-set evaluation, Logistic Regression achieved an ROC-AUC of 0.743, LDA achieved 0.727, and QDA achieved 0.677. After tuning, QDA achieved a test ROC-AUC of 0.782. These results are specific to the current data split and should not be interpreted as clinical validation.

## Limitations
The dataset is small and comes from a single source. The models are intended for educational and research purposes only and are not suitable for clinical decision-making.

## Author
Anantika Sisodiya
Avika Manglick 
Ishita Singh
