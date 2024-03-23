> #  Retail Sales Predictions
### Problem Statement
Rossmann operates over 3,000 drug stores in 7 European countries. Rossmann store managers are currently tasked with predicting their daily sales up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied. You are provided with historical sales data for 1,115 Rossmann Stores, The task is to forecast the "Sales" column for the test set. Note that some Stores in the dataset were temporarily closed for refurbishment.
### Summary
   Data from Rossman Stores has been provided to us, and it contains several variables that have an impact on the stores' sales. We'll talk about the project overview here.
   After outlining our problem statement, we started by gathering our data, which included loading datasets from importing libraries, checking for duplicate values (neither dataset contained any), and checking 
   for null values (none in the Store dataset but some in the Rossman dataset). Then, we learned how to interpret our variables, which also included their descriptions and unique values. Then, we moved on to Data 
   Wrangling, which involves handling null values by looking for outliers. Second, two datasets were combined. After that, we typecast.


### Datasets
Rossmann Stores Data.csv - historical data including Sales
Store.csv - supplemental information about the stores

> Rossmann Stores Data
  1. Store
  2. DayOfWeek
  3. Date
  4. Sales
  5. Customers
  6. Open
  7. Promo
  8. StateHoliday
  9. SchoolHoliday

> Store
  1. Store
  2. StoreType
  3. Assortment
  4. CompetitionDistance
  5. CompetitionOpenSinceMonth
  6. CompetitionOpenSinceYear
  7. Promo2
  8. Promo2SinceWeek
  9. Promo2SinceYear
  10. PromoInterval

#### ALGORITHMS USED:
I. Linear Regression, III. Decision Tree, IV. Ensemble Of Random forest.

#### Steps:
 1. Understanding Variable
 2. Data Wrangling
 3. Handling Outliers
 4. Categorical Encoding
 5. Feature Manipulation & Selection
 6. Data Transformation
 7. Data Scaling
 8. Data Splitting
 9. ML Model Implementation

> # Conclusion
### EDA Conclusion
We originally performed EDA on each feature of our dataset over the course of our investigation. Sales, our dependent variable, was first analyzed and converted. Next, we examined categorical variables and eliminated those that were dominated by a single class. We also examined numerical variables and used the corr() Function to determine their correlation, distribution, and relationship to the dependent variable. Finally, for multicollinearity, we used the VIF Function that we had developed. Additionally, we hot-encoded the categorical variables and deleted several numerical characteristics with a large percentage of 0 values.

As my observation Sales are highest during the three months of the year i.e., July, November and December and the least sales are during the month of May.
Sales increase year by year because stores give discounts on products.
When School is closed Some stores sales drop but B type of store does not affect sales when the school opens or closes.
Mostly Sales of B type of Assortment (Extra things).
Sales are maximum during the Public Holidays, where are during the religious occassions, like Easter or Christmas, the sales are lower , most of sales of B type assortment of all Holiday.
As my ovservation the highest sales belonged to the store type A due to the high number of type a stores in our dataset. Store type a and c had a similar kind of sales and customer share.

### Conclusion Ml Models: 
We Used three types of Machin learning algorithm for best prediction Linear Regressions, Decision Tree and Hyperparmeter techniques.

First we start with Linear Regression we have approx 70% accuracy and R2 0.82 on test data but this is not upto the mark. So for more accuracy we moved further with more complex model i.e., Decision Tree.

On test data, this model has an almost 94% accuracy rate or R2 0.95 , which is better than the linear regression model. But in order to ensure your happiness, we also ran a Random Forest Regressor model.

We achieved around 95% accuracy or R2 0.96 on test data with our model, which is an improvement over the prior model.

The best outcome is being produced by the Random Forest Regresson. So, in order to forecast our model, we will utilize Random Forest Regressor.






