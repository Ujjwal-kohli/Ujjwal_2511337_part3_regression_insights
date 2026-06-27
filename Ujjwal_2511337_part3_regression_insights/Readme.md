# Task 1 – Understand the Dataset

## Objective

The objective of this task is to understand the dataset before performing regression analysis by identifying the target variable, potential predictor variables, data types, and any preprocessing requirements.

## Dependent Variable (Target)

* **monthly_sales**

This is the target variable that the regression model will predict.

## Potential Independent Variables (Predictors)

The following variables may influence monthly sales and will be considered as independent variables:

* marketing_spend
* footfall
* avg_discount_pct
* staff_count
* inventory_availability_pct
* competitor_distance_km
* holiday_flag
* customer_rating
* region
* store_type

## Numerical Variables

* marketing_spend
* footfall
* avg_discount_pct
* staff_count
* inventory_availability_pct
* competitor_distance_km
* customer_rating
* monthly_sales
* monthly_profit

## Categorical Variables

* region
* store_type

These variables must be encoded before fitting a regression model.

## Binary Variable

* holiday_flag

This variable contains two possible values (0 = No Holiday, 1 = Holiday) and can be used directly in regression after validating that only binary values exist.

## Variables That May Need Cleaning or Transformation

* Check for missing values in all columns.
* Remove duplicate records if any exist.
* Verify that **holiday_flag** contains only valid binary values (0 or 1).
* Check numerical variables for outliers, especially:

  * marketing_spend
  * footfall
  * monthly_sales
  * monthly_profit
* Standardize categorical values in **region** and **store_type** if inconsistent.
* Encode categorical variables (dummy variables or one-hot encoding) before regression.
* Review numerical variables for extreme values and transform them if required.

## Variables That May Not Be Useful for Regression

* **store_id**

  * This is a unique identifier for each store and does not explain sales performance.
* **month**

  * If stored as text, it cannot be used directly in regression. It should either be transformed into useful time-based features (such as month number or season) or excluded if time effects are not part of the analysis.
* **monthly_profit**

  * Since the objective is to predict **monthly_sales**, this variable should not be used as an independent variable because it is an outcome measure that is closely related to sales and may introduce data leakage.

## Summary

The regression model will use **monthly_sales** as the dependent variable and evaluate the impact of marketing, customer traffic, discounts, staffing, inventory availability, competition, holidays, customer ratings, store type, and region on monthly sales performance. Proper data cleaning, validation, and encoding will be completed before model development.



# Regression Approach

The analysis started with simple linear regression to understand the relationship between monthly sales and one independent variable at a time. After that, a multiple regression model was developed using several independent variables together to understand their combined effect on monthly sales.

---

# Dummy Variable Approach

The categorical variables **store_type** and **region** were converted into dummy variables before running the multiple regression model.

For **store_type**, the **Residential** category was used as the reference category, and dummy variables were created for High Street, Mall, and Airport.

For **region**, the **West** category was used as the reference category, and dummy variables were created for North, South, and East.

The reference categories were excluded from the regression model to avoid the dummy variable trap.

---

# Model Comparison Summary

Eight simple regression models and one multiple regression model were compared.

Among the simple regression models, **Footfall (R² = 0.7363)** and **Staff Count (R² = 0.6523)** had the strongest relationship with monthly sales.

The Multiple Regression model performed the best with:

* R² = 0.8570
* Adjusted R² = 0.8504
* Standard Error = 40133.89

This model explains about **85.7%** of the variation in monthly sales and provides better predictions than the individual simple regression models.

---

# Final Model Selected

The **Multiple Regression Model** was selected as the final model because it achieved the highest R² value and considers the combined effect of multiple business factors. It is more suitable for predicting monthly sales and supporting business decisions.

---

# Business Recommendation

Based on the regression analysis, the company should focus on increasing customer footfall, maintaining adequate staff, improving inventory availability, and continuing effective marketing activities. Business decisions should also consider differences in store type and region when planning future strategies.

---

# Assumptions and Limitations

* The analysis is based on historical data.
* Regression identifies relationships between variables but does not prove cause and effect.
* Some important factors, such as weather, local events, competitor promotions, and customer behaviour, were not included in the dataset.
* The model should be used as a decision-support tool along with business knowledge.

---

# Screenshots Included

* simple_regression_output.png
* multiple_regression_output.png
* model_comparison_preview.png
* residuals_preview.png
