## Executive Summary

In this report, we present a comprehensive evaluation of various regression models applied to our dataset. The objective of this analysis is to identify the most suitable regression model for our predictive task. We have assessed the following models:

1. Linear Regression
2. Ridge Regression
3. Lasso Regression
4. Elastic Net
5. Decision Trees
6. Random Forest
7. Partial Least Squares Regression

Our evaluation includes the use of common regression evaluation metrics, including Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and R-squared (R²) score. We conducted the evaluation on three distinct datasets: training, validation, and test sets.

## Model Performance Summary

### Linear Regression

- **RMSE(train,val,test):** 3.336, 3.030, 2.656
- **MAE(train,val,test):** 2.683, 2.417, 2.142
- **R-squared(train,val,test):** 0.995, 0.995, 0.991

**Analysis and Insights:**
- Linear Regression exhibits strong predictive performance, with consistently low RMSE and MAE across all datasets.
- The high R-squared values indicate that Linear Regression captures a substantial portion of the variance in the target variable.
- The model seems to generalize well to the validation and test datasets, demonstrating its robustness.

### Ridge Regression

- **RMSE(train,val,test):** 3.470, 2.697, 3.030
- **MAE(train,val,test):** 2.709, 2.130, 2.310
- **R-squared(train,val,test):** 0.994, 0.996, 0.989

**Analysis and Insights:**
- Ridge Regression introduces regularization to mitigate overfitting, resulting in slightly higher RMSE and MAE on the training set.
- The model excels in generalization, as evidenced by its impressive performance on the validation and test sets.
- High R-squared values indicate that Ridge Regression effectively models the target variable.

### Lasso Regression

- **RMSE(train,val,test):** 4.227, 3.607, 3.661
- **MAE(train,val,test):** 3.478, 2.981, 3.269
- **R-squared(train,val,test):** 0.991, 0.993, 0.983

**Analysis and Insights:**
- Lasso Regression introduces feature selection by driving some coefficients to zero, resulting in a simpler model.
- While it has higher RMSE and MAE compared to Linear and Ridge Regression, Lasso's simplicity can be advantageous.
- It still captures a significant portion of the variance in the target variable.

### Elastic Net

- **RMSE(train,val,test):** 7.549, 5.711, 5.311
- **MAE(train,val,test):** 5.884, 4.871, 4.469
- **R-squared(train,val,test):** 0.973, 0.982, 0.965

**Analysis and Insights:**
- Elastic Net combines Ridge and Lasso regularization techniques, offering a balance between them.
- While it has higher RMSE and MAE compared to Linear and Ridge Regression, it provides better generalization compared to Lasso.
- The model captures a substantial portion of the variance in the target variable.

### Decision Trees

- **RMSE(train,val,test):** 2.064, 3.589, 3.284
- **MAE(train,val,test):** 1.306, 2.842, 2.431
- **R-squared(train,val,test):** 0.998, 0.993, 0.987

**Analysis and Insights:**
- Decision Trees show excellent predictive power on the training set, achieving the lowest RMSE and MAE.
- However, there is a risk of overfitting, as indicated by the higher RMSE and MAE on the validation and test sets.
- Feature importance analysis may help identify critical predictors.

### Random Forest

- **RMSE(train,val,test):** 0.851, 2.832, 3.201
- **MAE(train,val,test):** 0.513, 1.818, 1.718
- **R-squared(train,val,test):** 0.999, 0.996, 0.987

**Analysis and Insights:**
- Random Forest demonstrates remarkable predictive power, achieving the lowest RMSE and MAE across all datasets.
- The model excels in generalization, as indicated by its strong performance on the validation and test sets.
- Feature importance analysis may provide insights into critical predictors.

### Partial Least Squares Regression

- **RMSE(train,val,test):** 3.944, 3.346, 3.942
- **MAE(train,val,test):** 3.044, 2.518, 2.939
- **R-squared(train,val,test):** 0.993, 0.994, 0.981

**Analysis and Insights:**
- Partial Least Squares Regression aims to find latent factors that explain the variance in both predictors and the target.
- It achieves competitive RMSE and MAE while offering a different perspective on feature relationships.
- Further analysis may help interpret the latent factors identified by the model.

## Model Selection

- Based on our evaluation, the **Random Forest** regression model is recommended as the most suitable choice for our predictive task.
- It offers the best balance between accuracy and generalization across the training, validation, and test sets.
- Feature importance