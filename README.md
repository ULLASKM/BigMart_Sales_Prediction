# Sales Prediction for Big Mart Outlets

### Using LGBM Regressor
#### LB - https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/#LeaderBoard
#### Public Rank - TOP 3%

The data scientists at BigMart have collected 2013 sales data for 1559 products across 10 stores in different cities. Also, certain attributes of each product and store have been defined. The aim is to build a predictive model and predict the sales of each product at a particular outlet.
Using this model, BigMart will try to understand the properties of products and outlets which play a key role in increasing sales.
Please note that the data may have missing values as some stores might not report all the data due to technical glitches. Hence, it will be required to treat them accordingly. 

#### Model Approach

1) Data Pre-Processiing and Feature Engineering:

   a) Merging Same categories into common names
   
   b) Imputing Missing Values with custom method¶
   
   c) Imputing 0's in Item_Visibility with Mean values
   
   d) New Feature generation
   
   e) Converting established_date to Age(Years) of the outlet
   
   f) Quantile based binning for Item_weight
   
   g) Label Encoding categorical features
   
2) Splitting up train and test Data
3) Training LGBM Model with K-fold for CV
4) Evaluation of Model using RMSE
5) Model Interpretation and Analysis using SHAP
6) Feature Selection based on SHAP
7) Fitting the model again with cleaned data.
8) Predition on Test dataset.
9) Submission
        

#### Evaluation Metric

We at our end, have the actual sales for the test dataset, against which your predictions will be evaluated. We will use the Root Mean Square Error value to judge your response.

#### Model Interpretation and Analysis using SHAP

![Alt text](https://github.com/ULLASKM/BigMart_Sales_Prediction/blob/master/Shap_Summary_Plot.png "Shap Summary Plot")
![Alt text](https://github.com/ULLASKM/BigMart_Sales_Prediction/blob/master/Shap_WaterFall_Plot.png "Shap Waterfall Plot")
