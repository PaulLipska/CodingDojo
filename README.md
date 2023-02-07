# Sales as a Function of Item Weight
## The Heavy Cost of Large Items 

**Paul Lipska**: 

### Business problem:

Maximizing Sales

### Data:
Sales data from 1998 - 2009

### Data Dictionary

![alt text](https://github.com/PaulLipska/Food-Sales-Predictions/blob/main/Data_Dictionary.PNG)

## Methods
- Data was cleaned and missing values were imputed
- Duplicate values were resolved 

## Results
- Two problem areas were Item_Weight and Outlet_Size.  For the first we chose to impute the median value and for the latter we replaced Nan values with "missing"
- The result of our first investigation shows a possible relation between weight of an item and its sales potential, see graph below.

#### Distrobution of Sales by Weight of Item Sold
![alt text](https://github.com/PaulLipska/Food-Sales-Predictions/blob/main/Hist_wt.png)

> You can see the vast majority of sales is for items weighing 12.5 lbs.  You can see sales per unit decreases from the extreme left to extreme right.

## Model

Models used:
### Linear Regression Model

Regression Model Train Scores
* MAE: 849.1725 
* MSE: 1304275.8163 
* RMSE: 1142.049 
* R2: 0.5592852

Regression Model Test Scores
* MAE: 803.8961 
* MSE: 1192541.2373 
* RMSE: 1092.0354 
* R2: 0.5677597

### Decision Tree Regressor Model

High Bias Decision Tree Model Train Scores
* MAE: 1138.5329 
* MSE: 2255705.5459 
* RMSE: 1501.9006 
* R2: 0.2377972

High Bias Decision Tree Model Test Scores
* MAE: 1112.1494 
* MSE: 2125288.2422 
* RMSE: 1457.8368 
* R2: 0.2296826

You can see the R^2 for the Linear Regression Model matched 60% of the training data

## Recommendations:
Looking at supermarket types you can see a relationship between sales and store type.  Does this prove or refute the thesis of this exploration?
A further review of sales by store type and by item weight might provide more insights and new directions.
![alt text](https://github.com/PaulLipska/Food-Sales-Predictions/blob/main/sales_type.png)

## Limitations & Next Steps
Can we retreive the missing values for a more complete exploration?  Another item to consider in relations to weight of items is the cost of freight, logistics and wharehousing. A good place to start testing changes would be on the lowest performing supermarket type.  The changes would be immediately relevant and could be measured with minimal negative affect.


### For further information


For any additional questions, please contact **paul.lipska@gmail.com**
