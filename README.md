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


## Exploratory Data Analysis:
![image](https://user-images.githubusercontent.com/103464406/218009404-3930913f-3c55-4b36-a7fd-b83e1bc80b04.png)
- There are 5891 users in the dataset and 3631 uique products
- 31% of Product_Category_2 and 69% of Product_Category_3 has missing values.
![image](https://user-images.githubusercontent.com/103464406/218009159-c83bd506-4ff6-4634-b1c7-e57f827911b1.png)
![image](https://user-images.githubusercontent.com/103464406/218009176-bbb80aad-c939-47aa-aee2-ec0632fccf2b.png)
![image](https://user-images.githubusercontent.com/103464406/218008941-34dc24c1-cc6c-4a11-8464-bcd4a7915ee2.png)
![image](https://user-images.githubusercontent.com/103464406/218008902-7e533e3d-dd7b-4e97-a5de-63caef13f217.png)
![image](https://user-images.githubusercontent.com/103464406/218008959-c5f25aec-b153-41f6-a832-096b54905dc1.png)
![image](https://user-images.githubusercontent.com/103464406/218008979-6911cf5c-b129-496c-a5c5-0259b3ea366b.png)
![image](https://user-images.githubusercontent.com/103464406/218009029-9221bf47-b53e-4b32-a36e-0ef054141ce1.png)
![image](https://user-images.githubusercontent.com/103464406/218009042-89c50ed4-cee5-4515-bfe1-124687d8eac7.png)
![image](https://user-images.githubusercontent.com/103464406/218009295-86f598f7-ed23-4b7d-a2a6-11f89aea1102.png)
![image](https://user-images.githubusercontent.com/103464406/218009337-43927dfc-6185-41c3-962d-3b76682ab88f.png)
![image](https://user-images.githubusercontent.com/103464406/218009949-e9b19c79-a789-4adc-b7a0-6939ae67c797.png)


## Data Preprocessing:
  - Product category 2 and 3 has missing values, we will use SimpleImputer to fill missing values with median values.
  - Handle categorical columns Gender, Age, City_Category,Stay_In_Current_City_Years
## Modelling
