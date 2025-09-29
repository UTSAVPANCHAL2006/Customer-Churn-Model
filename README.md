Customer Churn Prediction

🌟 Overview:
Predict customer churn for a telecom company using historical data to identify at-risk customers and support proactive retention strategies.

📊 Dataset:
Telco Customer Churn Dataset (Kaggle)

Key Features

👤 Customer Info: gender, SeniorCitizen, Partner, Dependents

📅 Tenure

📞 Services: PhoneService, MultipleLines, InternetService

🔒 Security & Support: OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport

📺 Entertainment: StreamingTV, StreamingMovies

📄 Billing & Contract: Contract, PaperlessBilling

💳 Payments: PaymentMethod, MonthlyCharges, TotalCharges

🎯 Target: Churn

🛠️ Approach

Data preprocessing

Handle missing values (TotalCharges) ✅

One-hot encode categorical variables 🏷️

Scale numeric features (Tenure, MonthlyCharges, TotalCharges) 📏

Modeling

Logistic Regression ⚡

Random Forest Classifier 🌲

Evaluation Metrics

Accuracy, Precision, Recall, F1-score, ROC AUC 📈

Feature Importance (Random Forest)

Features with importance > 0.100 are the strongest predictors of churn:

TotalCharges 💰

Total customer spend. Longer-term or high-spending customers churn less.

Tenure ⏳

Customer lifetime. Shorter-tenure customers are more likely to churn.

MonthlyCharges 💳

Recurring monthly fees. Higher charges often increase churn risk, especially for month-to-month contracts.

Contract 📄

Contract type (Month-to-month, 1-year, 2-year). Month-to-month customers have the highest churn risk.

Insight:
These four features dominate predictions, showing churn is mainly driven by tenure, spending behavior, and contract type. Other features (<0.100 importance) contribute less but can still provide minor insights.
