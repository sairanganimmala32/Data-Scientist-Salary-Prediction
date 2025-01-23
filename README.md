# Data-Scientist-Salary-Prediction

## Project Overview
• Created a machine learning model that **estimates salary of data scientist based on the features like rating, company_founded, etc.**<br/>
• Engineered features from the text of each job description to quantify the value companies put on python, excel, tableau and sql


## Exploratory Data Analysis (EDA) and Data Cleaning
• **Removed unwanted columns**: 'Unnamed: 0'<br/>
• **Plotted bargraphs and countplots** for numerical and categorical features respectively for EDA<br/>
![image](https://github.com/user-attachments/assets/c7d86605-7fed-4447-9fa8-8cedad7c6fd3)     ![image](https://github.com/user-attachments/assets/28be6b78-1e03-48ce-83a1-2dd8613fe9dd)



• **Numerical Features** (Rating, Founded): **Replaced NaN or -1 values with mean or meadian based on their distribution**<br/>
• **Categorical Features: Replaced NaN or -1 values with 'Other'/'Unknown' category**<br/>
• **Removed unwanted alphabet/special characters from Salary feature**<br/>
• **Converted the Salary column into one scale** i.e from (per hour, per annum, employer provided salary) to (per annum)

## Feature Engineering
• **Creating new features** from existing features e.g. **job_in_headquaters from (job_location, headquarters)**, etc.<br/>
• **Trimming columns**  having more than 10 categories to **reduce the dimensionality**<br/>
• **Handling ordinal and nominal categorical features**<br/>
• **Feature Selection** using **information gain (mutual_info_regression) and correlation matrix**<br/>
![image](https://github.com/user-attachments/assets/d07f97e9-fb10-4e0c-b6f2-3b7043002155)


![image](https://github.com/user-attachments/assets/7866caf3-7c45-4c5f-a00f-bf370fdaed9c)


•  Feature Scaling using **StandardScalar**

## Model Building and Evaluation
Metric: Negative Root Mean Squared Error (NRMSE)<br/>
Linear regression: -28.82889464163559
Lasso regression: -28.905978321919985
RandomForest: -19.091528460060285
GradientBoosting: -25.278672413039576

_**Note: Evaluation scores are obtained using cross validation.**_
