
# Advanced House Price Prediction - Kaggle Competition

## Overview

This project aims to predict house prices using a comprehensive dataset from the [Advanced House Price Regression competition on Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques). The dataset contains various features, such as property characteristics and sale prices, allowing us to build a robust regression model to predict house values.

## Objective

The main goal of this project is to apply regression techniques to predict the sale price of houses. By leveraging different machine learning algorithms and feature engineering techniques, we aim to minimize the prediction error (RMSE) on the test dataset.

## Dataset

The dataset consists of:

- **Training Data**: Contains 1460 observations with 80 features each, including numerical and categorical variables.
- **Test Data**: Includes the same features as the training set, minus the target variable (SalePrice).
- **Target Variable**: `SalePrice` (House price in dollars).

Key features include:

- **Numerical Features**: LotArea, YearBuilt, GrLivArea, etc.
- **Categorical Features**: Neighborhood, HouseStyle, etc.

## Approach

1. **Data Preprocessing**:
   - Handle missing values.
   - Impute numerical and categorical data.
   - Encode categorical variables.

2. **Feature Engineering**:
   - Explore feature interactions.
   - Select important features using techniques such as Mutual Information (MI) and Principal Component Analysis (PCA).

3. **Modeling**:
   - Train Gradient Boosting Regressor
   - Evaluate model performance using cross-validation.

4. **Model Tuning**:
   - Optimize model hyperparameters to improve accuracy.
   - Use techniques such as Grid Search for tuning.

## Evaluation Metric

The competition uses **Root Mean Squared Error (RMSE)** as the evaluation metric. The formula for RMSE is:

```
RMSE = sqrt(mean((y_true - y_pred)²))
```

## Results

The model's performance is evaluated based on RMSE. Key results include:

- **Best Model**:
```
   GradientBoostingRegressor(learning_rate=0.01, max_depth=5, max_features='sqrt', min_samples_leaf=2, min_samples_split=10, n_estimators=1000, subsample=0.8)
```
  
- **Best RMSE on Validation Set**: 0.12398
- **Techniques Used**: Feature Engineering, Regularization, Ensemble Methods, etc.

## Conclusion

This project demonstrates the application of advanced regression techniques to predict house prices. Future improvements could include deeper feature engineering, more complex model architectures, or ensembling multiple models for better accuracy.

## Acknowledgments

- Kaggle for hosting the competition and providing the dataset.
