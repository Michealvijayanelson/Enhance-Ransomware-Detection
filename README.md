Ransomware Detection Using Integrated Ensemble Learning and Dimensionality Reduction
📌 Project Overview
This project implements an advanced machine learning pipeline for ransomware detection.
It uses feature selection, SMOTE oversampling, PCA dimensionality reduction, and ensemble models to classify ransomware vs. benign activities with high accuracy.

🎯 Objective
To detect ransomware attacks efficiently by:

Reducing feature dimensions to improve speed and accuracy

Balancing imbalanced datasets using SMOTE

Comparing multiple machine learning models

🗂 Dataset
File: ransomware_detection_updated.csv

Contains system log records with numerical features

Label column: Ransomware Label (1 = Ransomware, 0 = Benign)

⚙️ Workflow
Data Preprocessing

Keep only numerical columns

Drop missing values

Feature Selection

SelectKBest with Mutual Information to select top 25 features

Scaling

StandardScaler for normalization

Class Balancing

SMOTE with sampling strategy 0.8

Dimensionality Reduction

PCA to reduce features to a maximum of 10 components

Train-Test Split

75% training, 25% testing, stratified on label

Model Training

Random Forest (with hyperparameter tuning)

XGBoost (with hyperparameter tuning)

LightGBM (with hyperparameter tuning)

Logistic Regression

Evaluation

Accuracy score

Confusion matrix

Classification report

ROC curve

Model comparison bar chart

📊 Models Used
Random Forest Classifier

XGBoost Classifier

LightGBM Classifier

Logistic Regression

📈 Results
Accuracy comparison of all models

Confusion matrix heatmaps

ROC curve with AUC score for each model

🛠 Tech Stack
Language: Python

Libraries:

numpy

pandas

scikit-learn

imbalanced-learn

xgboost

lightgbm

matplotlib

seaborn
