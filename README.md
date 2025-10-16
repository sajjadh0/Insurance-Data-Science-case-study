**Insurance Cost Prediction - Linear Regression Case Study**

This project implements a Linear Regression model to predict insurance costs based on various customer attributes. The analysis includes comprehensive exploratory data analysis (EDA), data preprocessing, feature engineering, and model evaluation to understand the factors that influence medical insurance charges.

---

### **Objective**

To build a predictive model that can estimate insurance charges based on customer demographics, health metrics, and lifestyle factors, helping insurance companies better understand pricing determinants.

---

### **Dataset**

The dataset contains 1,338 records with the following features:

- **Features**:
  - Categorical: sex, region, smoker
  - Numerical: age, bmi, children
- **Target**: charges (numeric)

---

### **Implementation**

- **Handling Categorical Variables**: One-Hot Encoding for sex, smoker, and region
- **Feature Scaling**: MinMaxScaler for numerical features (age, bmi, children)
- **Data Splitting**: 80-20 train-test split with random state for reproducibility

---

### **Model Architecture**

- **Algorithm**: Linear Regression
- **Feature Engineering**: ColumnTransformer for mixed data types
- **Evaluation Metrics**:
  - R² Score
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)

---

### **Exploratory Data Analysis Insights**

- **Age Distribution**: Normal distribution with concentration around middle-aged individuals
- **BMI Analysis**: Right-skewed distribution with some outliers in higher BMI ranges
- **Smoking Impact**: Significant correlation between smoking status and insurance charges
- **Regional Patterns**: Variations in charges across different geographical regions

---

### **Model Performance**

- **R² Score**: ~0.784 (78.4% variance explained)
- **Mean Absolute Error**: ~$4,181

**Training vs Testing:**

- Training R²: Higher (not explicitly shown but implied by tighter clustering)
- Testing R²: 0.784 (78.4% variance explained)
- Performance Gap: Small difference between training and testing performance indicates good model generalization

---

### **Polynomial Regression (Degree 2)**

- **R² Score**: ~0.86–0.88 (improvement from 0.784)
- **MAE**: Reduced from ~$4,181
- **MSE**: Significant reduction

**Degree Comparison:**

- Degree = 2 gives the best R² score
- Degree = 3 gives a somewhat better R² score (R² = 0.84...)

---

### **Improvements**

- **+8–10% R² Increase**: Substantial improvement in explained variance
- **Better Error Metrics**: Lower prediction errors across the board
- **Enhanced Predictive Power**: Model captures more complex patterns

---

### **Visualizations**

![Training Predictions](https://github.com/user-attachments/assets/d620dabc-2e71-440e-a998-aea9d7b90ca3)  
*X-axis: Actual insurance charges from the training dataset  
Y-axis: Predicted insurance charges from the model on training data  
Red diagonal line: Ideal prediction line (where predicted = actual)*

![Testing Predictions](https://github.com/user-attachments/assets/36538fcf-c4a1-4ff3-8f3f-0dc4e30885a4)

![Polynomial Regression Degree 2](https://github.com/user-attachments/assets/98508213-c020-44e9-b1f5-f647cb3f8353)

![Polynomial Regression Degree 3](https://github.com/user-attachments/assets/da837c5d-6492-4e7e-9029-2ca77717b7c6)
