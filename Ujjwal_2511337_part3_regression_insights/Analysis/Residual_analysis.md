# Residual Analysis

The final multiple regression model was used to predict monthly sales for each store.

Predicted sales were calculated using the regression equation, and residuals were calculated using the formula:

**Residual = Actual Sales − Predicted Sales**

A positive residual means the actual sales were higher than the predicted sales. A negative residual means the actual sales were lower than the predicted sales.

## Top 5 Largest Positive Residuals

| Predicted Sales |   Residual |      Residual² |
| --------------: | ---------: | -------------: |
|      759,919.94 | 111,017.46 | 12,324,876,541 |
|      610,531.95 | 103,079.21 | 10,625,323,212 |
|      721,415.92 |  91,900.79 |  8,445,755,202 |
|      701,381.34 |  86,334.17 |  7,453,589,490 |
|      540,234.62 |  85,279.42 |  7,272,579,252 |

These stores performed better than the model predicted. This may be because of factors that were not included in the model, such as local promotions, better store management, customer preferences, or seasonal demand.

## Top 5 Largest Negative Residuals

| Predicted Sales |    Residual |      Residual² |
| --------------: | ----------: | -------------: |
|      764,038.71 | -136,866.81 | 18,732,523,948 |
|      805,279.85 | -119,900.77 | 14,376,194,966 |
|      709,913.78 | -114,446.18 | 13,097,927,103 |
|      912,344.87 | -111,892.93 | 12,520,027,901 |
|      808,021.71 |  -86,942.36 |  7,558,973,864 |

These stores performed worse than the model predicted. Possible reasons include lower customer demand, stock shortages, stronger local competition, operational issues, or other factors that were not included in the dataset.

## Business Interpretation

The residual analysis shows that the multiple regression model predicts monthly sales fairly well for most stores. However, a few stores have large positive or negative residuals, which means there are additional business factors affecting sales that are not captured in the model.

Stores with large **positive residuals** were **under-predicted**, meaning their actual sales were higher than expected.

Stores with large **negative residuals** were **over-predicted**, meaning their actual sales were lower than expected.

Overall, the model is useful for predicting monthly sales, but it should be used along with business knowledge because regression shows relationships based on the available data and cannot capture every real-world factor that affects store performance.
