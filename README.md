# 📊 ElasticNet Regression 

This project implements **ElasticNet Regression**, a hybrid regularization technique combining **Lasso** (L1) and **Ridge** (L2) regularization. ElasticNet is particularly useful when dealing with datasets with correlated features and helps with both regularization and feature selection.

## 🛠 Tools & Libraries Used

- **Python 🐍**
- **Pandas** & **NumPy** (Data manipulation and numerical computations)
- **Matplotlib** & **Seaborn** (Data visualization)
- **Scikit-learn** (Model building, evaluation, and hyperparameter tuning)

---

## 🔑 What is ElasticNet?

- **ElasticNet** combines both **L1 (Lasso)** and **L2 (Ridge)** penalties to improve regression models.
- It is particularly effective when:
  - The number of predictors (features) is larger than the number of observations.
  - There are correlations among features.
- ElasticNet can be controlled using two parameters:
  - `alpha`: Regularization strength.
  - `l1_ratio`: Controls the mix between Lasso (L1) and Ridge (L2). 
    - `l1_ratio = 1` corresponds to Lasso.
    - `l1_ratio = 0` corresponds to Ridge.

---

## ⚙️ Steps Involved

1. **Creating and Explore the Data**
   - Creating dataset using `pandas`
   - Visualize relationships between features and the target variable

2. **Preprocessing**
   - Handle missing values
   - Encode categorical features
   - Normalize or standardize features to improve model performance
   - Split the data into training and test sets

3. **ElasticNet Regression**
   - Train an ElasticNet model using `sklearn.linear_model.ElasticNet`
   - Tune the `alpha` and `l1_ratio` parameters using cross-validation
   - Evaluate model performance using R² score, MAE, and MSE

4. **Visualization**
   - Plot coefficients as a function of `alpha` and `l1_ratio`
   - Compare ElasticNet with Lasso and Ridge on various metrics

