# Customer Churn Prediction using Machine Learning

## Project Overview

Customer churn is an important business problem where companies need to identify customers who are likely to stop using their services.

This project analyzes customer data and develops machine learning models to predict customer churn. The project includes data cleaning, exploratory data analysis (EDA), feature engineering, machine learning classification, model evaluation, SHAP-based explainability, and Power BI reporting.

The project was completed as part of a Business Analytics internship project.

---

## Objectives

- Analyze customer data to identify churn patterns.
- Clean and preprocess the dataset.
- Perform exploratory data analysis (EDA).
- Identify important factors associated with customer churn.
- Build machine learning classification models.
- Evaluate and compare model performance.
- Use SHAP to explain model predictions.
- Present analytical findings through Power BI.

---

## Dataset

The project uses the Telco Customer Churn dataset.

### Dataset Information

- Total records: 7,043
- Churned customers: 1,869
- Retained customers: 5,174
- Churn rate: approximately 26.5%

The dataset contains customer demographic information, account information, service details, and churn status.

---

## Project Workflow

```text
Data Collection
      ↓
Data Cleaning
      ↓
Data Preprocessing
      ↓
Exploratory Data Analysis
      ↓
Feature Engineering
      ↓
Train-Test Split
      ↓
Machine Learning Models
      ↓
Model Evaluation
      ↓
SHAP Explainability
      ↓
Power BI Dashboard
      ↓
Business Insights

**Data Cleaning and Preprocessing**

The dataset was prepared for analysis by:

Checking for missing values
Handling inconsistent data types
Converting numerical and categorical variables
Encoding categorical variables
Preparing the target variable
Removing or handling unsuitable records
Preparing features for machine learning

**Exploratory Data Analysis**

Exploratory Data Analysis (EDA) was performed to understand customer behavior and identify patterns associated with churn.

The analysis examined relationships between churn and factors such as:

Contract type
Monthly charges
Customer tenure
Payment method
Internet service
Customer services
Demographic characteristics
Account-related attributes

Visualizations were created to understand distributions, relationships, and differences between churned and retained customers.

**Feature Engineering**
Feature engineering was performed to prepare relevant variables for machine learning.

The process included:

Selecting relevant features.
Transforming categorical variables.
Encoding categorical variables.
Preparing numerical features.
Creating a machine-learning-ready dataset.
Machine Learning Models

Three classification models were developed and evaluated:

Logistic Regression
Random Forest
XGBoost

These models were used to identify patterns associated with customer churn and generate churn predictions.

**Model Evaluation**

The models were evaluated using multiple classification metrics:

Accuracy
Precision
Recall
F1-Score
ROC-AUC

Using multiple evaluation metrics provides a broader view of model performance, particularly for a classification problem where both retained and churned customers need to be considered.

Model Performance
Logistic Regression
Accuracy: 79.84%
Precision: 65.00%
Recall: 52.14%
F1-Score: 57.86%
ROC-AUC: 0.8423
XGBoost
ROC-AUC: 0.8443

Detailed model evaluation results are available in:

Model_Performance.csv
Explainable AI with SHAP

SHAP (SHapley Additive exPlanations) was used to improve the interpretability of the machine learning model.

SHAP analysis was used to understand:

Which features have a stronger influence on churn predictions.
How individual features affect model predictions.
The relative importance of customer attributes.
Factors associated with higher or lower predicted churn.

The SHAP feature importance results are available in:

SHAP_Feature_Importance.csv
Power BI Dashboard

A Power BI dashboard was created to present the customer churn analysis in an interactive format.

The dashboard provides insights into:

Overall customer churn
Customer segmentation
Churn patterns
Customer characteristics
Contract and service-related patterns
Key analytical findings

The data prepared for Power BI is available in:

Customer_Churn_PowerBI.csv
Key Insights

The analysis was used to investigate:

Which customer segments have higher churn rates.
How customer tenure is related to churn.
How contract type is associated with customer retention.
How monthly charges are associated with churn behavior.
Which customer features contribute to churn predictions.
Which factors may be useful for identifying customers at risk of churn.

These insights can support further customer retention analysis and help businesses identify areas requiring additional investigation.

Technologies Used
Programming
Python
Data Analysis
Pandas
NumPy
Data Visualization
Matplotlib
Seaborn
Power BI
Machine Learning
Scikit-learn
XGBoost
Explainable AI
SHAP
Development Tools
Jupyter Notebook
Git
GitHub
Skills Demonstrated

This project demonstrates practical experience in:

Data Cleaning
Data Preprocessing
Data Validation
Exploratory Data Analysis
Feature Engineering
Quantitative Data Analysis
Machine Learning
Classification
Model Evaluation
Explainable AI
SHAP Analysis
Data Visualization
Power BI
Data Interpretation
Business Analytics
Data Reporting

**How to Run the Project**

1. Clone the repository
git clone https://github.com/Samikshya981/customer-churn-prediction-ml.git
2. Navigate to the project directory
cd customer-churn-prediction-ml
3. Install the required Python libraries
pip install -r requirements.txt
4. Start Jupyter Notebook
jupyter notebook
5. Open the notebook

Open:

Customer_Churn_Prediction_Analysis.ipynb

Run the notebook cells sequentially to reproduce the analysis.

Reproducibility

The project includes the Python notebook and supporting result files used during the analysis.

The requirements.txt file lists the major Python dependencies required for the project.

For reproducibility, ensure that the required Python libraries are installed before running the notebook.

Business Use Case

Customer churn prediction can help organizations identify customers who may be at higher risk of leaving a service.

A churn analysis workflow can support:

Customer retention analysis
Customer segmentation
Identification of churn-related patterns
Data-driven decision-making
Targeted retention strategies
Business performance monitoring

The predictions generated by this project are intended for analytical and educational purposes and would require additional validation before being used in a production environment.

**Limitations**
The analysis is based on the available dataset and its underlying assumptions.
Model performance may vary with different datasets and customer populations.
Additional feature engineering and model tuning could potentially improve performance.
Production deployment would require additional validation, monitoring, and testing.
Business decisions should not be based solely on model predictions.
**Future Improvements**

Possible future improvements include:

Hyperparameter tuning.
Cross-validation.
Additional machine learning algorithms.
Handling class imbalance using appropriate techniques.
Model monitoring.
Deployment as a web application or API.
Automated data pipelines.
Automated model retraining.
Integration with real-time customer data.
Development of an automated churn reporting system.
