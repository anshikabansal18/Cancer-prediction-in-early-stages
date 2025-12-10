# 🩺 Cancer Risk Prediction Using Machine Learning

A comprehensive machine learning project designed to predict cancer risk levels using lifestyle, environmental, medical, and genetic features. This project includes full data analysis, multiple ML models, interpretability tools, interactive UI, and research-grade evaluation techniques.

## 📂 Dataset Overview

The dataset contains 1000 patient records with 25 features representing:

- Demographics (Age, Gender)

- Lifestyle factors (Smoking, Alcohol Use, Balanced Diet)

- Environmental exposure (Air Pollution, Occupational Hazards)

- Medical history (Chronic Lung Disease, Obesity, Genetic Risk)

- Symptoms (Chest Pain, Shortness of Breath, Fatigue, etc.)

### ✔ Data Cleaning Performed

- Removed Patient Id column (not useful for ML)

- Converted categorical values to numeric representations

- Verified no missing values, ensuring dataset integrity

## 🔍 Exploratory Data Analysis (EDA)

EDA was performed using:

### ✔ Countplots & histograms

To study distribution of smoking, pollution, gender, symptoms, etc.

### ✔ Heatmaps

To identify correlations between environmental, lifestyle, and genetic factors.

### ✔ Boxplots

Revealed insights such as:

- Age distribution vs chest pain

- Smoking levels across risk groups

- Pollution vs genetic predisposition

### Key Observations

- Smoking and pollution scores increase with cancer risk.

- GeneticRisk is highly correlated with Level.

- Age shows clusters, especially around 30–40 years.

## 🤖 Machine Learning Models Implemented

The following models were trained and evaluated:

- Random Forest Classifier

- Support Vector Classifier (SVC)

- K-Nearest Neighbors (KNN)

- Decision Tree Classifier

- XGBoost Classifier

- LightGBM Classifier

All models were evaluated using:

- Accuracy

- F1 Score

- Log Loss

- ROC-AUC Score

 <img width="468" height="199" alt="Screenshot 2025-12-10 at 2 45 50 PM" src="https://github.com/user-attachments/assets/0e2c628e-48d8-4a28-91b1-e3c8b496770d" />

## 📈 ROC Curves

ROC curves were plotted for all models, showing:

- Almost perfect AUC scores due to strong separability in dataset

- Ensemble models performed the best (RF, XGBoost, LightGBM)

- SVC achieved strong performance but lacks predict_proba support in some kernels

## 🧠 Model Interpretability (Explainability)
### ✔ SHAP Global Feature Importance

Shows which factors contribute most to cancer risk predictions.

Top Predictors Identified:

- GeneticRisk

- Smoking

- AirPollution

- PassiveSmoker

- Chronic Lung Disease

### ✔ SHAP Summary Plots

Helped visualize each feature’s effect on predictions.

## 🧪 Learning Curves (Overfitting Analysis)

Learning curves were generated for:

- Random Forest

- SVC

- KNN

- Decision Tree

- XGBoost

- LightGBM

### Insights:

- Decision Trees show slight overfitting

- Random Forest generalizes well after SMOTE

- KNN slightly underfits

- XGBoost and LightGBM show excellent convergence

## 🏁 Conclusion

This project provides:

- A complete ML pipeline

- Clear visualizations

- Multiple tuned models

- Robust evaluation (AUC, Log loss, F1 Score)

- Interpretability with SHAP
