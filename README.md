# 📊 Experiment 2: Loan Amount Prediction using Linear Regression

This project is part of the **Machine Learning Algorithms Laboratory (ICS1512)** for **M.Tech (Integrated) CSE, Semester V** at **Sri Sivasubramaniya Nadar College of Engineering**.

## 🎯 Objective

Build and evaluate a **Linear Regression** model using Scikit-learn to predict the **loan sanction amount** for users based on various demographic and financial features.

---

## 🗂️ Folder Contents

```
.
├── Linear_Regression.ipynb         # Jupyter Notebook implementation
├── report.tex                      # LaTeX report file (Experiment 2)
├── report.pdf                      # Final compiled PDF report
├── train.csv                       # Dataset (from Kaggle)
├── loan_distribution.png           # Plot 1: Histogram
├── heatmap.png                     # Plot 2: Correlation heatmap
├── actualvspred.png                # Plot 3: Actual vs Predicted
├── Residual_distribution.png       # Plot 4: Residual plot
├── coefficient.png                 # Plot 5: Feature coefficients
└── README.md                       # This file
```

---

## 🧪 Steps Performed

### 1. Data Preprocessing
- Removed null and invalid loan entries
- Selected relevant features
- Encoded categorical variables using `OrdinalEncoder`
- Standardized features using `StandardScaler`

### 2. Model Building
- Applied **Linear Regression** using `sklearn.linear_model.LinearRegression`
- Applied **log transformation** to the target variable
- Evaluated using:
  - MAE
  - MSE
  - RMSE
  - R² and Adjusted R²

### 3. Validation
- Performed 5-Fold Cross Validation using `KFold`
- Reported average metrics

### 4. Visualizations
- Distribution of loan amounts
- Feature correlation heatmap
- Actual vs predicted values
- Residual distribution
- Feature importance coefficients

---

## 📈 Results

| Metric             | Value         |
|--------------------|---------------|
| MAE (Test Set)     | 15,157.87     |
| MSE (Test Set)     | 1.81e9        |
| RMSE (Test Set)    | 42,511.29     |
| R² Score           | 0.0636        |
| Adjusted R²        | 0.0539        |
| CV Avg R² (K=5)    | 0.8458        |

---

## 🧠 Learning Outcomes

- Understood real-world data preprocessing and cleaning
- Learned to use Linear Regression for prediction
- Applied log transformation for skewed data
- Validated models using K-Fold cross-validation
- Visualized predictions and residuals

---

## 📚 References

- [scikit-learn: Linear Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)
- [Kaggle Dataset](https://www.kaggle.com/datasets/phileinsophos/predict-loan-amount-data)
- [Seaborn Documentation](https://seaborn.pydata.org/)
