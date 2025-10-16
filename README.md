**Insurance Cost Prediction - Linear Regression Case Study**

This project implements a Linear Regression model to predict insurance costs based on various customer attributes. The analysis includes comprehensive exploratory data analysis (EDA), data preprocessing, feature engineering, and model evaluation to understand the factors that influence medical insurance charges.

**Objective**

To build a predictive model that can estimate insurance charges based on customer demographics, health metrics, and lifestyle factors, helping insurance companies better understand pricing determinants.


**DataSet**
dataset contains 1,338 records with the following features
Features: (categorical- sex, region, smoker)
          (numerical- age, bmi, children)
Target: charges(numeric)


**Implementation** 

->Handling Categorical Variables: One-Hot Encoding for sex, smoker, and region

->Feature Scaling: MinMaxScaler for numerical features (age, bmi, children)

->Data Splitting: 80-20 train-test split with random state for reproducibility

**Model Architecture**

Algorithm: Linear Regression

Feature Engineering: ColumnTransformer for mixed data types

Evaluation Metrics:

R² Score

Mean Absolute Error (MAE)

Mean Squared Error (MSE)





