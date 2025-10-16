**Insurance Cost Prediction - Linear Regression Case Study**

This project implements a Linear Regression model to predict insurance costs based on various customer attributes. The analysis includes comprehensive exploratory data analysis (EDA), data preprocessing, feature engineering, and model evaluation to understand the factors that influence medical insurance charges.

**Objective**                                                           

To build a predictive model that can estimate insurance charges based on customer demographics, health metrics, and lifestyle factors, helping insurance companies better understand pricing determinants.


**DataSet**                                                                                      
Dataset contains 1,338 records with the following features
->Features: (categorical- sex, region, smoker)
          (numerical- age, bmi, children)                                            
->Target: charges(numeric)


**Implementation**                                                                               

->Handling Categorical Variables: One-Hot Encoding for sex, smoker, and region
->Feature Scaling: MinMaxScaler for numerical features (age, bmi, children)
->Data Splitting: 80-20 train-test split with random state for reproducibility


**Model Architecture**
Algorithm: Linear Regression
->Feature Engineering: ColumnTransformer for mixed data types                                    
->Evaluation Metrics:                                                  
->R2 Score                                                                      
->Mean Absolute Error (MAE)                                        
->Mean Squared Error (MSE)                                                                       

**Exploratory Data Analysis Insights**                                        
->Age Distribution: Normal distribution with concentration around middle-aged individuals
->BMI Analysis: Right-skewed distribution with some outliers in higher BMI ranges
->Smoking Impact: Significant correlation between smoking status and insurance charges
->Regional Patterns: Variations in charges across different geographical regions

**Model Performance**                                                  
->R2 Score: ~0.784 (78.4% variance explained)                                        
->Mean Absolute Error: ~$4,181                                                                  






**Polynomial Regression (Degree 2):**                                                  
Performance metrics for polynomial features                                                  
->R2 Score: ~0.86-0.88 (improvement from 0.784)                
->MAE: Reduced from ~$4,181                                                                      
->MSE: Significant reduction   
<img width="457" height="571" alt="Screenshot 2025-10-14 105014" src="https://github.com/user-attachments/assets/98508213-c020-44e9-b1f5-f647cb3f8353" />
**Deegree= 2 gives the best r2 score**


<img width="462" height="568" alt="Screenshot 2025-10-14 105032" src="https://github.com/user-attachments/assets/da837c5d-6492-4e7e-9029-2ca77717b7c6" />
**Degree=3 gives some what better r2 score**                
R2 score= 0.84...

**Improvements:**
-> +8-10% R2 Increase: Substantial improvement in explained variance
->Better Error Metrics: Lower prediction errors across the board
->Enhanced Predictive Power: Model captures more complex patterns



