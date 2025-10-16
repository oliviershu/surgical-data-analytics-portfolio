# Surgical Site Infection (SSI) Prediction – Summary

This project builds a baseline machine-learning model to predict the likelihood of postoperative surgical site infection (SSI) using structured variables such as age, BMI, operative time, and comorbidity indicators.  
A synthetic dataset of 300 observations was generated to simulate typical peri-operative characteristics.

A simple logistic regression model achieved a test accuracy of **≈85–90%** depending on seed variation, demonstrating feasibility for early-stage risk modeling.  
Next steps include extending to Random Forest and XGBoost for comparison, plotting ROC and precision-recall curves, and generating SHAP interpretability plots to identify the most influential predictors.

The notebook and folder structure follow a reproducible research pattern—datasets in `/data`, code in `/notebooks`, and output plots in `/reports/figures`.
**Results:** On synthetic peri-operative data (n≈300), RandomForest and XGBoost modestly outperformed Logistic Regression by ROC AUC (~0.02–0.08). Precision–recall was consistent with class balance. SHAP highlighted operative time, BMI>30, and diabetes as the strongest contributors. (Exact values vary with the random seed; code is fully reproducible.)
