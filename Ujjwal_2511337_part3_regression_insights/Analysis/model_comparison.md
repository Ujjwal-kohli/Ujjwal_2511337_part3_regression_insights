# Model Comparison

## Simple Regression Equations

Simple regression was used to understand how one factor at a time affects monthly sales.

General equation:

**Monthly Sales = Intercept + (Coefficient × Independent Variable)**

Examples:

* Monthly Sales = Intercept + (1.2099 × Marketing Spend)
* Monthly Sales = Intercept + (27.3362 × Footfall)
* Monthly Sales = Intercept + (-41243.15 × Average Discount %)
* Monthly Sales = Intercept + (3508.40 × Staff Count)
* Monthly Sales = Intercept + (3062.21 × Inventory Availability %)
* Monthly Sales = Intercept + (-3438.11 × Competitor Distance)
* Monthly Sales = Intercept + (15157.29 × Holiday Flag)
* Monthly Sales = Intercept + (12509.46 × Customer Rating)

---

# Multiple Regression Equation

Monthly Sales =

66915.47

* (1.2099 × Marketing Spend)

* (27.3362 × Footfall)

− (41243.15 × Average Discount %)

* (3508.40 × Staff Count)

* (3062.21 × Inventory Availability %)

− (3438.11 × Competitor Distance)

* (15157.29 × Holiday Flag)

* (12509.46 × Customer Rating)

* (20219.26 × High Street)

* (32832.85 × Mall)

* (44695.09 × Airport)

− (15342.71 × North)

− (4201.85 × South)

− (25291.42 × East)

---

# Explanation of Coefficients

* **Marketing Spend:** More marketing is generally linked with higher sales.
* **Footfall:** More customers visiting the store usually leads to higher sales.
* **Average Discount %:** A higher discount is linked with lower sales in this model after considering other variables.
* **Staff Count:** Stores with more staff generally have better sales.
* **Inventory Availability %:** Better product availability helps improve sales.
* **Competitor Distance:** Stores closer to competitors may have lower sales.
* **Holiday Flag:** Sales usually increase during holidays.
* **Customer Rating:** Better customer ratings are linked with higher sales.

---

# Dummy Variables

Two categorical variables were converted into dummy variables.

### Store Type

Reference Category: **Residential**

Dummy variables created:

* High Street
* Mall
* Airport

Residential was used as the reference category. The coefficients show how each store type performs compared with Residential stores.

### Region

Reference Category: **West**

Dummy variables created:

* North
* South
* East

West was used as the reference category. The coefficients compare the sales performance of other regions with the West region.

---

# Final Model Selected

The **Multiple Regression Model** was selected as the final model.

### Reason for Selecting the Final Model

The multiple regression model gave the best performance with an **R² value of 0.8570**. This means it explains about **85.7% of the variation in monthly sales**. It also considers several business factors together instead of looking at only one factor at a time. Because of this, it gives a more complete picture and is more useful for business decision-making.
