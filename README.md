# Health Insurance Premium Prediction
# Introduction
This project aims to develop a machine learning model that predicts the annual health insurance premium a customer needs to pay based on key factors such as age, health status, income, and lifestyle habits. The insurance industry relies on risk assessment models to determine fair and competitive pricing for customers while ensuring profitability. However, traditional methods can be inefficient, inconsistent, and prone to human bias.

By analyzing demographic attributes (age, gender, marital status, and region), health-related factors (BMI, smoking status, and medical history), and financial details (income level, employment status, and insurance plan type), this model helps insurance companies automate premium calculation and optimize risk management.

The predictive model ensures that premiums are set fairly and accurately, reducing the likelihood of undercharging high-risk customers or overcharging low-risk individuals. This improves customer satisfaction, encourages affordable policy offerings, and enhances business efficiency by reducing manual effort in premium estimation.

Additionally, the project can be extended to dynamic premium adjustments, where policyholders can receive revised premium estimates based on their lifestyle changes. The insights from this model can also help insurance companies design better policies by understanding risk patterns across different customer segments.

# dataset Description
The dataset contains various attributes influencing insurance premium calculations. The key features are:

Input Features:

Demographics:

age: Age of the customer

gender: Male/Female

region: Location of the customer

marital_status: Single/Married

number_of_dependents: Number of dependents on the policyholder

Health-Related Factors:

bmi_category: Body Mass Index category (Underweight, Normal, Overweight, Obese)

smoking_status: Smoker/Non-smoker

medical_history: Previous health conditions

Financial & Employment Information:

employment_status: Employed/Self-employed/Unemployed

income_level: Low/Middle/High

income_lakhs: Income of the customer in lakhs

insurance_plan: Type of insurance plan chosen

Target Variable:

annual_premium_amount: The premium amount a customer needs to pay annually (Predicted Value).

# Handling Missing Values
* The dataset had missing values in **smoking_status (11), employment_status (2), and income_level (13)**, which were dropped to ensure data quality. This helps maintain model accuracy by avoiding               
inconsistencies caused by null values.
* There is no duplicated data.

# Data Cleaning
* We can see some negative values in number_of_dependants. We can replace them with positive numbers

# Univariate Analysis: Numeric Columns
*The dataset analysis revealed the presence of outliers in the 'Age' and 'Income' columns, which may impact the overall statistical analysis and model performance.

![image](https://github.com/user-attachments/assets/0ffc1fd4-8f3a-4466-b3d9-2b9ab3bfcd2e)

![image](https://github.com/user-attachments/assets/046a6b73-764f-4a1e-b6da-abbb3c1f0c2f)

The **outliers** in the dataset have been addressed as follows:

***Age Column**: All records where age exceeds 100 have been removed to maintain data integrity.

***Income Column**: Instead of using the IQR method, which would remove many legitimate records, we opted for a quantile-based threshold approach. After discussions with the business team, we selected the 0.999 quantile, which corresponds to an income threshold of 100 lakhs.

![image](https://github.com/user-attachments/assets/5e58c4c0-bbb8-48bc-9e8b-717a054c9def)

*Most individuals are young (20–30 years) with fewer older customers.
*Many people have no dependents, but a significant portion has 1–3 dependents.
*Income is highly skewed, suggesting income disparities among customers.
*Annual premium payments follow a similar pattern to income, with a majority in the lower range





    








