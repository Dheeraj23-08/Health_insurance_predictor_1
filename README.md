Insurance Premium Prediction and Customer Segmentation
This project focuses on predicting annual insurance premium amounts and segmenting customers based on various demographic, health, and financial attributes. The goal is to build robust machine learning models that can accurately estimate premiums and identify distinct customer groups, which can be valuable for personalized insurance product offerings and risk assessment.

Project Overview
The project involves a comprehensive data science workflow, including:

Data Loading and Exploration: Initial understanding of the dataset structure and content.

Data Preprocessing and Cleaning: Handling missing values, removing duplicates, and treating outliers to ensure data quality.

Feature Engineering and Transformation: Preparing categorical and numerical features for model training.

Customer Segmentation: Dividing the customer base into meaningful groups using clustering techniques.

Machine Learning Model Development: Building and evaluating regression models for premium prediction.

Dataset
The dataset contains the following features:


Age: Age of the customer.

Gender: Gender of the customer.

Region: Geographical region of the customer.

Marital_status: Marital status of the customer.

Number Of Dependants: Number of dependents the customer has.

BMI_Category: Body Mass Index category (e.g., Normal, Overweight, Obesity, Underweight).

Smoking_Status: Smoking habits (e.g., No Smoking, Regular, Occasional).

Employment_Status: Employment type (e.g., Salaried, Self-Employed, Freelancer).

Income_Level: Income range (e.g., <10L, 10L - 25L, 25L - 40L, > 40L).

Income_Lakhs: Income in Lakhs (numerical).

Medical History: Pre-existing medical conditions (e.g., Diabetes, High blood pressure, Heart disease, Thyroid, No Disease).

Insurance_Plan: The customer's insurance plan (Bronze, Silver, Gold).

Annual_Premium_Amount: The annual premium paid by the customer (target variable).

Methodology
Data Preprocessing
Column names were standardized by replacing spaces with underscores and converting to lowercase.


Missing values in 

smoking_status, employment_status, and income_level were removed.


Duplicate records were identified and removed.


Outliers in 

age (values greater than 100) and income_lakhs (values above the 99.9th percentile) were handled by filtering the data.


Negative values in 

number_of_dependants were converted to their absolute values.


Customer Segmentation
The project includes notebooks (codebasics_data_segmentation.ipynb, data_segmentationss.ipynb) that likely perform customer segmentation based on various features. This involves identifying natural groupings within the customer data to understand different customer personas.

Premium Prediction Models
Separate premium prediction models were developed, potentially for different customer segments:

Overall Premium Prediction: Using Linear Regression, Ridge, and Lasso models.

Segment-specific Prediction:


premium_rest.xlsx - Sheet1.csv: Data for the 'rest' segment.


premium_young.xlsx - Sheet1.csv: Data for the 'young' segment (customers with age <= 25).

Dedicated notebooks (

code_ml_premium_prediction_rest.ipynb, ml_pred_rest.ipynb, code_ml_premium_prediction_young.ipynb, ml_pred_young.ipynb) were used for these segments, applying similar data cleaning and modeling techniques.


Model Evaluation
The models were evaluated using standard regression metrics:


R-squared (R2 Score)

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

Mean Absolute Error (MAE)

Cross-validation (GridSearchCV, RandomizedSearchCV) was also utilized for hyperparameter tuning and robust model evaluation.


How to Use
Clone the Repository:

Bash

git clone <repository-url>
Install Dependencies:
Make sure you have Python installed. Then, install the required libraries:

Bash

pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
Run Jupyter Notebooks:
Navigate to the project directory and open the Jupyter notebooks:

Bash

jupyter notebook
You can then run the cells in each notebook to see the data analysis, segmentation, and model predictions.

Files in the Repository
before_segment.ipynb: Initial data loading, cleaning (missing values, duplicates, age/dependents outliers).

code_ml_premium_prediction.ipynb: Comprehensive notebook covering overall data loading, EDA, cleaning, and application of Linear Regression, Ridge, and Lasso models.

code_ml_premium_prediction_rest.ipynb: Focuses on premium prediction for the 'rest' customer segment.

code_ml_premium_prediction_young.ipynb: Focuses on premium prediction for the 'young' customer segment.

codebasics_data_segmentation.ipynb: Likely contains the core code for customer segmentation.

data_segmentationss.ipynb: Another notebook related to data segmentation.

ml_pred_rest.ipynb: Possibly an alternative or refined version of premium prediction for the 'rest' segment.

ml_pred_young.ipynb: Possibly an alternative or refined version of premium prediction for the 'young' segment.

premium_rest.xlsx - Sheet1.csv: Dataset for the 'rest' customer segment.

premium_young.xlsx - Sheet1.csv: Dataset for the 'young' customer segment.

Dependencies
pandas

numpy

matplotlib

seaborn

scikit-learn

statsmodels