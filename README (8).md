#  Telco-Customer-Churn-Pipeline
End-to-End Machine Learning Pipeline for predicting customer churn using Logistic Regression and Random Forest with GridSearchCV hyperparameter tuning and production-ready pipeline export.


## Objective
Build a reusable and production-ready machine learning pipeline to predict customer churn using the Telco Churn dataset.

## Methodology / Approach
1. **Data Preprocessing:**  
   - Handle missing values  
   - Convert `TotalCharges` to numeric  
   - Encode categorical variables using `OneHotEncoder`  
   - Scale numerical features using `StandardScaler`  
   - Built preprocessing pipelines using `ColumnTransformer`  

2. **Modeling:**  
   - Trained **Logistic Regression** and **Random Forest** using Scikit-learn Pipeline API  
   - Tuned hyperparameters using **GridSearchCV** with cross-validation  

3. **Evaluation:**  
   - Used **accuracy, precision, recall, F1-score** for performance evaluation  
   - Selected the best model (Random Forest) based on metrics  

4. **Export:**  
   - Saved final pipeline using `joblib` for reusability and deployment  

## Key Results / Observations
- Logistic Regression Accuracy: ~78.96%  
- Random Forest Accuracy: ~78.82%  
- Dataset is imbalanced; recall for churn class is low (~50%)  
- Both pipelines are reusable and production-ready  
- Further tuning or class balancing could improve churn detection
