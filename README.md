# Urinary-Cancer Survial Classification
Urinary Cancer Classification using Hybrid Ensemble and Explainable AI

📘 Project Overview

This project presents a machine learning pipeline for urinary cancer classification using the SEER dataset. It integrates hybrid feature selection (ANOVA + RFE), ensemble learning models (LightGBM, CatBoost, TabNet), and explainable AI (SHAP & LIME) techniques. The framework aims to enhance predictive performance, interpretability, and clinical reliability in urinary cancer survival classification.

🚀 Key Features

Data Preprocessing

      Missing values imputed using RandomForestRegressor and RandomForestClassifier
      
      Categorical encoding via LabelEncoder and OneHotEncoder
      
      Feature scaling using StandardScaler

Feature Selection

      Dual-stage hybrid method combining ANOVA (filter-based) and RFE (wrapper-based)
      
      Selection of statistically significant and model-relevant features

Base Models

Logistic Regression

      Naïve Bayes
      
      Random Forest
      
      Decision Tree
      
      LightGBM
      
      CatBoost
      
      XGBoost

Proposed Stacked Ensemble

      Base learners: LightGBM, CatBoost, TabNet
      
      Meta-learner: Logistic Regression
      
      Optimized using GridSearchCV and cross-validation

Model Evaluation Metrics

      Accuracy, Precision, F1-Score, ROC–AUC
      
      Matthews Correlation Coefficient (MCC) — emphasizes balanced performance across classes

Explainable AI

      SHAP (global interpretability): identifies dominant predictive features
      
      LIME (local interpretability): provides case-level rationale

📂 Dataset

      Source: SEER Urinary Cancer Dataset (SEER_URINARY.csv)
      
      Target variable: STAT_REC (cancer status)
      
      Data Access: A sample of 20 anonymized records has been included in this repository to demonstrate the dataset structure and preprocessing workflow.

                  Due to the ICMR–NIRT data protection policy, the complete dataset is restricted and cannot be publicly shared. The datasets used and/or analysed during the current study are available from the corresponding author upon reasonable request, strictly for academic and research purposes.
