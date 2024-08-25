# Lasso Regression Hyperparameter Tuning

This repository demonstrates how to perform hyperparameter tuning for a Lasso Regression model using Python. The tuning is done manually with `GridSearchCV` rather than using the `lassoCV` API. The example uses the Boston Housing dataset to predict housing prices.

## Overview

Lasso Regression is a type of linear regression that includes a regularization term. This term penalizes the absolute size of the regression coefficients, effectively shrinking some coefficients to zero. This can be useful for feature selection and improving model interpretability.

In this project, we:
- Load and preprocess the data using pandas.
- Split the data into training and testing sets.
- Train a Lasso Regression model.
- Manually tune the hyperparameters using `GridSearchCV` to find the best regularization parameter (`alpha`).
- Evaluate the model's performance using the R² score.

## Dependencies

- Python 3.x
- pandas
- scikit-learn

## Results

- **Initial Model**: The R² score without tuning the hyperparameters.
- **Optimized Model**: The R² score after tuning the hyperparameters using `GridSearchCV`, resulting in a better fit compared to the initial model.

## Conclusion

This example highlights the importance of hyperparameter tuning in improving the performance of machine learning models. By manually tuning the `alpha` parameter, the Lasso Regression model achieved a better R² score, indicating a more accurate model.
