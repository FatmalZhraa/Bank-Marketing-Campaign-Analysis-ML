# 📌 Bank Marketing Prediction & Segmentation
## 📖 Overview

This project analyzes the Bank Marketing Dataset (Kaggle) to predict whether a client will subscribe to a term deposit.
The goal is to help banks optimize marketing campaigns by focusing on the most promising clients.

## 🎯 Business Problem

Banks spend significant resources calling clients during marketing campaigns.
However:

Many clients are unlikely to subscribe → wasted time & cost.

Random calling annoys customers and reduces efficiency.

👉 Using Machine Learning, we predict subscription probabilities and segment clients into high, medium, and low potential.

## 📊 Dataset

Source: Bank Marketing Dataset (Kaggle)

Rows: ~41k clients

Target variable: y → Did the client subscribe? (yes / no)

Features:

Demographics: age, job, education, marital status

Financial: housing loan, personal loan, default

Campaign: contact method, previous outcome, campaign calls

Economic Indicators: euribor3m, employment variation rate, etc.

## ⚙️ Approach
1. Data Preprocessing

Removed duplicates

Dropped irrelevant columns (duration)

Train/test split (70/30)

Applied StandardScaler for numeric & OneHotEncoder for categorical

2. Exploratory Data Analysis (EDA)

Subscription rates by age, education, job

Trends over month & weekday

Impact of contact methods & previous outcomes

3. Modeling

Logistic Regression → interpretable baseline

Random Forest → feature importance + better performance

Evaluation metrics: Accuracy, Precision, Recall, F1-score

4. Segmentation

Using predict_proba instead of simple Yes/No:

High Probability (>0.7) → Focus in campaigns

Medium Probability (0.4–0.7) → Follow-up needed

Low Probability (<0.4) → Not priority

## 📈 Business Value

✅ Save campaign costs
✅ Improve ROI by targeting high-potential clients
✅ Reduce unnecessary calls (better customer experience)
✅ Provide insight dashboards (Power BI) for managers

🛠️ Tools & Libraries

Python: Pandas, Matplotlib, Seaborn, Scikit-learn

Models: Logistic Regression, Random Forest

Visualization: Power BI Dashboard

## Dashboard

![bank dashboard](https://github.com/user-attachments/assets/aae3ffc6-0158-4d86-98f1-fb9c6ad8ec50)

## 📌 Results

Logistic Regression Accuracy: ~89%

Random Forest Accuracy: ~88%

Business segmentation insights generated
