Customer Churn Prediction Model 🚀
Overview
This project aims to predict customer churn for a telecommunications company. By analyzing demographic data, account information, and service usage, the model identifies customers at high risk of leaving the service. The goal is to provide actionable insights for retention teams.

Tech Stack
Language: Python

Libraries: Pandas, NumPy, Scikit-Learn, Imbalanced-Learn, Joblib, Matplotlib, Seaborn

Methodology
Data Cleaning: Handled missing values in TotalCharges and removed non-predictive identifiers like customerID.

Exploratory Data Analysis (EDA): Visualized trends between tenure, payment methods, and churn status.

Feature Engineering: Applied Label Encoding and One-Hot Encoding to convert categorical data into numerical features.

Handling Imbalance: Implemented SMOTE (Synthetic Minority Over-sampling Technique) to ensure the model effectively learns from the minority churn class.

Modeling & Tuning: Used a Random Forest Classifier, fine-tuned with GridSearchCV to optimize for Recall.

Results
Recall achieved: 73% (Successfully capturing nearly 3 out of 4 churners).

Key Insights: * Customers using Electronic Check as a payment method show a higher propensity to churn.

There is a clear correlation between lower tenure and higher churn risk.

Visualizations
<img width="549" height="547" alt="image" src="https://github.com/user-attachments/assets/7af0fe0f-aadb-479f-b893-194a554f5370" />

<img width="531" height="547" alt="image" src="https://github.com/user-attachments/assets/19e532eb-2836-4f05-92a5-5bcbb829478f" />

<img width="515" height="432" alt="image" src="https://github.com/user-attachments/assets/6be75023-6dbf-436f-b25d-8b6614994e39" />




Confusion Matrix
This matrix highlights the model's ability to minimize missed churners (False Negatives).

Usage
Clone the repository.

Install dependencies: pip install -r requirements.txt

Run the model training script: python churn_prediction.py

The trained model is saved as churn_model.pkl and can be loaded for predictions using joblib.
