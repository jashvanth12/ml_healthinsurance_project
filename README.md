Health Insurance Premium Prediction
**Introduction**
This project aims to predict the annual health insurance premium for customers based on various demographic, health, and financial attributes. The model helps insurance companies in determining fair and personalized premium rates, improving customer satisfaction, and optimizing risk assessment.

**Problem Statement**
Insurance companies determine premium amounts based on multiple factors, including age, health conditions, lifestyle, and financial background. Manually assessing these factors is time-consuming and may lead to inconsistent pricing.

The objective of this project is to build a machine learning model that accurately predicts a customer's annual premium amount, enabling insurers to offer competitive and fair pricing.

**Dataset Description**
The dataset contains various attributes influencing insurance premium calculations. The key features are:

Input Features:
**Demographics:**

**age**: Age of the customer

**gender**: Male/Female

**region**: Location of the customer

**marital_status**: Single/Married

**number_of_dependents**: Number of dependents on the policyholder

**Health-Related Factors:**

**bmi_category**: Body Mass Index category (Underweight, Normal, Overweight, Obese)

**smoking_status**: Smoker/Non-smoker

**medical_history**: Previous health conditions

**Financial & Employment Information:**

**employment_status**: Employed/Self-employed/Unemployed

**income_level**: Low/Middle/High

**income_lakhs**: Income of the customer in lakhs

**insurance_plan**: Type of insurance plan chosen

**Target Variable**:

**annual_premium_amount**: The premium amount a customer needs to pay annually (Predicted Value).

**Solution Approach**

**1. Data Preprocessing**

Handling missing values

Encoding categorical variables

Feature scaling

**2. Exploratory Data Analysis (EDA)**

Identifying correlations between features and premium amount

Visualizing distributions of key features

**3. Model Selection & Training**

Regression models used:

Linear Regression

Random Forest

XGBoost

Gradient Boosting

**4. Model Evaluation**

Metrics used:

RMSE (Root Mean Square Error)

MAE (Mean Absolute Error)

R² Score (Coefficient of Determination)
