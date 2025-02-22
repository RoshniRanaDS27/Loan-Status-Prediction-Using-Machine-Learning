# Loan-Status-Prediction-Using-Machine-Learning
![image](https://github.com/user-attachments/assets/75800798-e2d6-4e76-abc0-0827d5ef28e0)


### Overview 📋
This end-to-end machine learning project predicts loan approval status based on customer profiles. Built using Python and scikit-learn, it covers data preprocessing, feature scaling, model training, evaluation, and hyperparameter tuning. Additionally, a user-friendly GUI was developed for seamless user interaction.

# Project Workflow 🔧
1. Data Loading  
2. Exploratory Data Analysis (EDA)  
3. Data Cleaning & Missing Value Handling  
4. Feature Engineering (Encoding Categorical Features)  
5. Feature Scaling  
6. Model Training and Evaluation  
7. Hyperparameter Tuning  
8. Cross-Validation (K-Fold)  
9. Model Deployment & GUI Development

# App demo 
![image](https://github.com/user-attachments/assets/c1f7f706-5703-471e-9539-d34a0d575c95)  
#
![image](https://github.com/user-attachments/assets/c79197f0-4ecc-46f8-8e85-1dc2618c92dd)


### Input Category   
![image](https://github.com/user-attachments/assets/1d851b4c-3f62-4379-be69-d625ed9e34b0)



# Breakdown of Key Concepts in the Code
## 🔍 Feature Scaling  
- Approach: Implemented StandardScaler to standardize numerical features like income and loan amount.  
- Purpose: Essential for distance-based models such as Logistic Regression and SVC to ensure fair weight distribution among features.  
  
## 🏷️ Feature Encoding
- Approach: Utilized Label Encoding to transform categorical variables into numeric values for model compatibility.  
- Example Mappings:
  
"Yes" → 1, "No" → 0  
"Male" → 1, "Female" → 0  
"Urban" → 2, "Semi-Urban" → 1, "Rural" → 0  

## 🧪 K-Fold Cross Validation
- Approach: Applied 5-Fold Cross-Validation using cross_val_score for robust performance evaluation.  
- Purpose: Helps ensure the model generalizes well across unseen data, mitigating overfitting risks.

## ⚡ Hyperparameter Tuning
- Approach: Employed RandomizedSearchCV to optimize model hyperparameters.  
- Examples:  
  - Logistic Regression & SVC optimized for the C (regularization) parameter.  
- Outcome: Significant performance boost, especially for SVC and Random Forest models.

# Insights from the Project
## 🌟 Key Influencing Features  
- Credit History: The most critical factor influencing loan approval.  
- Income: Applicant and co-applicant incomes significantly impacted the decision-making process.  

## 📈 Model Performance  
Baseline Performance: Logistic Regression and SVC performed reasonably well but required tuning.  
- Post-Tuning Results:  
- Random Forest: Achieved the highest accuracy (~80%) after tuning.  
- SVC: Performance improved post-tuning but remained slightly behind Random Forest.

## 🧹 Missing Values Strategy
- Minimal Missing Data (<5%): Columns like gender and dependents were dropped.  
- Key Columns: Imputed columns such as self_employed and credit_history using the most frequent value (mode).

## ⚖️ Feature Scaling
Why It Mattered: Standardized features (income, loan amount, loan term) ensured no single feature dominated due to scale differences.

## 🔄 Cross-Validation Insights
Outcome: The 5-Fold Cross-Validation demonstrated that the Random Forest model generalizes effectively across various data splits, making it the top performer.






