# RetailSales--Prediction
- The goal of a retail purchase prediction is to accurately forecast the demand for products and services to better manage inventory, anticipate customer needs, and maximize profits. 
- By leveraging data-driven models and predictive analytics, retailers can accurately forecast future sales and make more informed business decisions.

## Problem Statement:
- Exploratory data analysis to understand customer buying pattern
- Build a regression model to predict purchase amount of customer against various products

### Tools used:
- Python, Pandas (data processing), Plotlyexpress,Sklearn

## Data:
The dataset has 550,069 rows and 12 columns
### Attributes:
| Column ID |         Column Name        | Data type |           Description           | Masked |
|:---------:|:--------------------------:|:---------:|:-------------------------------:|--------|
|     0     |           User_ID          |   int64   |      Unique Id of customer      | False  |
|     1     |         Product_ID         |   object  |       Unique Id of product      | False  |
|     2     |           Gender           |   object  |         Sex of customer         | False  |
|     3     |             Age            |   object  |         Age of customer         | False  |
|     4     |         Occupation         |   int64   |   Occupation code of customer   | True   |
|     5     |        City_Category       |   object  |         City of customer        | True   |
|     6     | Stay_In_Current_City_Years |   object  | Number of years of stay in city | False  |
|     7     |       Marital_Status       |   int64   |    Marital status of customer   | False  |
|     8     |     Product_Category_1     |   int64   |       Category of product       | True   |
|     9     |     Product_Category_2     |  float64  |       Category of product       | True   |
|     10    |     Product_Category_3     |  float64  |       Category of product       | True   |
|     11    |          Purchase          |   int64   |         Purchase amount         | False  |
