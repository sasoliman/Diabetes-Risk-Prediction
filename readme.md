## 📖 Overview

This repository presents an end-to-end machine learning pipeline for predicting **diabetes risk** using demographic, socioeconomic, lifestyle, and clinical characteristics obtained from the **CDC Behavioral Risk Factor Surveillance System (BRFSS)**.

The project demonstrates an industry-standard workflow including:

- Data preprocessing and feature engineering
- Exploratory data analysis (EDA)
- CatBoost model development
- Hyperparameter optimization using Optuna
- Model evaluation
- Model interpretation using SHAP 
- Reproducible project structure using Git and Conda

## 📁 Repository Structure

```text
Diabetes-Risk-Prediction/

├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_Data_Loading.ipynb
│   ├── 02_Data_Preprocessing.ipynb
│   ├── 03_Exploratory_Data_Analysis.ipynb
│   ├── 04_CatBoost_Model.ipynb
│   └── 10_SHAP_Model_Interpretation.ipynb
│
├── figures/
├── models/
├── results/
├── environment.yml
├── requirements.txt
└── README.md
```


## 🤖 Machine Learning

The predictive model was developed using **CatBoost**

### Model Development

- Stratified train-test split
- 5-fold stratified cross-validation
- Hyperparameter optimization using Optuna
- Automatic class balancing
- Early stopping
- Final model retraining using the optimal hyperparameters

## 📊 Model Evaluation

Model performance is assessed using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC


## 🔍 Explainable Artificial Intelligence (XAI)

Model interpretation is performed using **SHAP (SHapley Additive Explanations)**.

The repository includes:

- SHAP Summary Plot
- SHAP Feature Importance
- SHAP Dependence Plots
- SHAP Waterfall Plot
- SHAP Force Plot

These visualizations provide both global and patient-level explanations of the CatBoost model.