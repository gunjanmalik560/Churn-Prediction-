## Overview 
This project focuses on predicting customer churn using a collection of demographic, financial, and usage-related customer data. The goal is to identify customers who are likely to discontinue the service, enabling businesses to take preventive actions.

The project includes data exploration, preprocessing, feature engineering, visualization, and machine learning model development.

## Key Steps in the Project
 1. Data Loading

-Loaded multiple sheets from Customer_Churn_Data_Large.xlsx.
-Merged them into a single unified dataset.
-Performed initial inspection with:
info()
describe()
-Null value analysis

 2. Exploratory Data Analysis (EDA)

- Performed detailed EDA to understand factors influencing churn:
🔹 Univariate Analysis
      Age distribution
      Spending patterns
      Login frequency
-Service usage
🔹Bivariate Analysis
     Churn rate vs income level
     Spending vs churn
     Online engagement behavior

  -Category-wise churn (Gender, MaritalStatus, IncomeLevel)
🔹 Correlation Analysis
    Created a correlation heatmap for numerical variables to identify:

-Key predictors
    Relationships between behaviour & churn

3. Data Preprocessing

-Converted "Yes"/"No" churn labels to binary 1/0
-Handled missing values
-Treated outliers using the IQR method
-Standardized numerical features where needed

4. Feature Engineering

-Added meaningful new variables such as:
 AvgSpendPerLogin
 Helps capture spending behaviour relative to activity.

 Aggregated financial metrics
 Derived insights from total spending, frequency, and usage.

 These new features improved model performance and business interpretability.

5. Model Development

Built multiple predictive models including:
-Logistic Regression
-Random Forest
-Each model was trained, tested, and evaluated using industry-standard metrics.

6. Model Evaluation

Used metrics such as:
-Accuracy
-Precision
-Recall
-F1-Score
Confusion Matrix
-ROC-AUC Curve
The model with the best balance between recall (catching at-risk customers) and precision was selected.

Technologies Used

-Python
-Pandas, NumPy
-Matplotlib, Seaborn
-Scikit-learn
-Machine learning 
