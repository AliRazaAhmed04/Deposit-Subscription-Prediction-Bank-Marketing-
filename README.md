# Term Deposit Subscription Prediction (Bank Marketing)
**Objective**

The aim of this project is to predict whether a bank customer will subscribe to a term deposit (personal loan/offer) as a result of a marketing campaign. By understanding customer behavior, banks can better target their marketing campaigns and improve acceptance rates.

**Dataset**

Source: UCI Machine Learning Repository – Bank Marketing Dataset

Description: The dataset contains information about customers contacted during marketing campaigns by a Portuguese banking institution.

Size: ~45,000 records (subset used here: 11,162 rows)

Target Variable:

deposit → yes/no (customer subscribed to a term deposit)

**Features**

Demographics: age, job, marital, education

Financials: default, balance, housing, loan

Campaign Details: contact, day, month, duration, campaign, pdays, previous, poutcome

**Project Workflow**

- Data Loading & Exploration

- Loaded dataset using Pandas

- Basic statistics & missing values check

- Distribution plots for key features (Age, Job, Marital Status)

- Preprocessing

- Encoded categorical features using LabelEncoder

- Removed irrelevant columns (if any)

- Split dataset into train (80%) and test (20%) sets

- Model Training

  - Logistic Regression (sklearn.linear_model.LogisticRegression)

  - Random Forest Classifier (sklearn.ensemble.RandomForestClassifier)

- Model Evaluation

- Accuracy, Precision, Recall, F1-Score

- Confusion Matrix

- ROC Curve and AUC comparison between models

- Explainability

Used SHAP (SHapley Additive exPlanations) to explain predictions

Explained 5 sample predictions

Created feature importance summary plot

**Results**

Logistic Regression Accuracy: ~78%

Random Forest Accuracy: ~83% (typically higher)

**Key Insights**

Campaign duration strongly influences subscription

Age, job, and balance are also important features


ROC curve comparison

SHAP explanations for predictions
