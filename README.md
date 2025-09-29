Customer Churn Prediction
🌟 Overview

This project predicts customer churn for a telecom company using historical customer data. The goal is to identify customers likely to leave and enable proactive retention strategies.

📊 Dataset

Telco Customer Churn Dataset from Kaggle: Link

Key Features:

👤 gender, SeniorCitizen, Partner, Dependents

📅 tenure

📞 PhoneService, MultipleLines, InternetService

🔒 OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport

📺 StreamingTV, StreamingMovies

📄 Contract, PaperlessBilling

💳 PaymentMethod, MonthlyCharges, TotalCharges

🎯 Churn (target)
🛠️ Approach

Data Preprocessing

Handle missing values (TotalCharges) ✅

One-hot encode categorical variables 🏷️

Scale numeric features (tenure, MonthlyCharges, TotalCharges) 📏

Modeling

Logistic Regression ⚡

Random Forest Classifier 🌲

Evaluation Metrics

Accuracy, Precision, Recall, F1-score, ROC AUC 📈


