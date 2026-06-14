# Customer Churn analysis and prediction for a telecom company

## Overview
This project showcases likelihoodness of a customer churning based on analysis and SHapley Additive exPlanations (SHAP).
What is SHAP? SHAP explains exactly which features pushed the model higher or lower than the baseline.

In this project, instead of accuracy, the model was focussed on high recall. Why recall? Because, recall measures the likelihood of customers churning ["Out of all true events, how many did the model successfully find."]

## Dataset
The project uses the IBM telecom churn data with the following columns:

- customerID   
- gender
- SeniorCitizen
- Partner
- Dependents
- tenure              
- PhoneService        
- MultipleLines       
- InternetService     
- OnlineSecurity      
- OnlineBackup        
- DeviceProtection    
- TechSupport         
- StreamingTV         
- StreamingMovies     
- Contract            
- PaperlessBilling    
- PaymentMethod       
- MonthlyCharges      
- TotalCharges        
- Churn 

Where, Churn is the dependent variable (y) and rest are independent variable

## Training Process
Load and Pre process the data
Exploratory data analysis
Check recall of best classification model
Build the best classification model
Introduce SHAP

## Results
After thorough exploration of data, predicitve analysis, it is come to attention that logistic regression performed the best with 76% recall. That is, the model is predicting 76% of churners.

## Technologies used
- Logistic Regression
- Pandas
- matplotlib and seaborn
- SHapely Additive exPlanations (SHAP)
- Data Preprocessing

## Learning Outcomes
- Performed end-to-end machine learning workflow, including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and interpretation. 
- Learned how to handle categorical variables using encoding techniques.  
- Understood the impact of class imbalance and applied SMOTE oversampling to improve minority class prediction.   
- Compared multiple classification algorithms, including Logistic Regression, Decision Tree, Random Forest, and XGBoost.  
- Evaluated models using business-relevant metrics such as Recall, Precision, F1-Score, and Accuracy rather than relying solely on accuracy.  
- Gained practical experience in customer churn prediction and retention analytics.   
- Used SHAP (SHapley Additive exPlanations) to interpret model predictions and identify key churn drivers.    
- Learned how feature importance and model explainability can support business decision-making.   
- Developed skills in data visualization using Matplotlib and Seaborn for exploratory analysis.   

## Future Improvements
- Perform hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
- Create customer lifetime value (CLV) features.
- Build individual customer-level SHAP explanations.
- Build a web dashboard using Streamlit for real-time churn prediction.
- Recommend retention strategies based on churn probability.