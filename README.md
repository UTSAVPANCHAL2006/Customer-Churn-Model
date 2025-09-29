Customer Churn Prediction

🌟 Overview:
This project predicts customer churn for a telecom company using historical customer data. The goal is to identify customers likely to leave and enable proactive retention strategies.

📊 Dataset:
Telco Customer Churn Dataset from Kaggle


Key Features:

   👤 gender, SeniorCitizen, Partner, Dependents
   
   📅 tenure
   
   📞 PhoneService, MultipleLines, InternetService
   
   🔒 OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport
   
   📺 StreamingTV, StreamingMovies
   
   📄 Contract, PaperlessBilling
   
   💳 PaymentMethod, MonthlyCharges, TotalCharges
   
   🎯 Churn (target)
   
🛠️ Approach:

  Data Preprocessing
  
  Handle missing values (TotalCharges) ✅
  
  One-hot encode categorical variables 🏷️
  
  Scale numeric features (tenure, MonthlyCharges, TotalCharges) 📏

Modeling:

  Logistic Regression ⚡
  
  Random Forest Classifier 🌲
  
  Evaluation Metrics
  
  Accuracy, Precision, Recall, F1-score, ROC AUC 📈

  
Feature Importance Overview:

After training a Random Forest model to predict customer churn, we analyzed the contribution of each feature. Features with importance values above 0.100 were identified as the most significant predictors of churn. These top features are:

TotalCharges:
Represents the total amount a customer has spent.
Longer-term or high-spending customers tend to have lower churn risk.

Tenure:
Measures how long a customer has been with the company.
Customers with shorter tenure are more likely to churn.

MonthlyCharges:
Indicates the recurring monthly subscription fee.
Higher monthly charges are often associated with higher churn probability, especially for customers on month-to-month contracts.

Contract:

The type of contract (month-to-month, one-year, two-year).
Month-to-month customers have the highest churn risk, while long-term contracts reduce churn likelihood.

Insight:
These four features dominate the model’s predictions, with importance values above 0.100, suggesting that churn is primarily driven by customer tenure, spending behavior, and contract type. Other features in the dataset had lower importance (<0.100), contributing less to the prediction but potentially useful for minor interactions.



