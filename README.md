Bank Marketing Campaign Prediction Project

Project Overview

This project analyzes a real-world bank marketing dataset to understand customer behavior and predict whether a customer will subscribe to a term deposit. The goal is to help the bank improve its marketing strategy using data-driven insights.


Objectives:

* Perform Exploratory Data Analysis (EDA) to understand the data
* Build a machine learning model to predict customer subscription
* Compare multiple models and select the best one
* Provide actionable suggestions to improve marketing campaigns
  

Dataset Description:

The dataset contains information about:

* Customer details (age, job, marital status, education, etc.)
* Financial status (loan, housing, default)
* Campaign details (contact type, month, previous outcomes)
* Economic indicators (interest rate, employment rate, etc.)

Target Variable:

* `y` → Whether the customer subscribed (`yes` / `no`)


## ⚙️ Steps Performed

Data Loading:

* Imported dataset using Pandas
* Checked structure, size, and column types


Data Cleaning:

* Identified and handled `"unknown"` values
* Converted target variable (`yes` → 1, `no` → 0)
* Removed **`duration`** column to avoid data leakage
* Handled special values like `pdays = 999`


Exploratory Data Analysis (EDA):

* Analyzed distribution of features (age, job, etc.)
* Compared features with target variable (`y`)
* Identified important patterns such as:
     * Certain jobs and age groups have higher subscription rates
     * Previous campaign success increases likelihood of conversion
     * Visualized data using graphs (histograms, count plots, heatmaps)


Feature Engineering:

* Created new features (e.g., previous contact indicator)
* Separated categorical and numerical features
* Applied:
  * One-Hot Encoding for categorical variables
  * Standard Scaling for numerical variables


Model Building:

Built multiple machine learning models:

* Logistic Regression
* Random Forest
* Gradient Boosting

Used a Pipeline to combine preprocessing and modeling.


Model Evaluation:

Evaluated models using:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC

Compared all models and selected the best-performing one.


Model Comparison:

* Compared performance of all models
* Selected the model with the best balance between:
* Predictive accuracy
* Ability to handle imbalanced data


Key Insights:

* Customers with successful past campaigns are more likely to subscribe
* Too many calls reduce effectiveness (customer fatigue)
* Certain months and contact methods perform better
* Economic conditions influence customer decisions


Business Recommendations

* Target high-probability customers using model predictions
* Focus on customers with positive past interactions
* Limit excessive follow-up calls
* Optimize campaign timing (month/day)
* Personalize marketing based on customer profile


Tools & Technologies Used:

* Python
* Pandas & NumPy → Data processing
* Matplotlib & Seaborn → Data visualization
* Scikit-learn → Machine learning models & pipelines

Conclusion:

This project demonstrates how data analysis and machine learning can be used to improve marketing strategies. By identifying the right customers to target, the bank can increase conversion rates and reduce unnecessary costs.


How to Run:
 
1. Clone the repository
2. Open the Jupyter Notebook
3. Install required libraries
4. Run all cells step by step



