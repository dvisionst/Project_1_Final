# Food Sales Predictions
## Using Predictive Machine Learning Models
Author: Jose Flores

## Business problem:
Using data from Big Mart Sales in order to predict item outlet sales.

## Data:
Original data was downloaded from https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/.
This dataset has 12 different features and a total of 8523 entries. This problem is related to predictive modeling, and I'll be using the data to make a prediction.

## Methods
I chose to use a simple impuder and encoder instead of dropping rows because of the amount of missing values. 
The data set itself has 8523 entries. The amount of missing values were 1463 for item weight and 2410 for outlet size. 
In percentage values those two represent 17% for weight and 28% for outlet size. 
I believe that is way too much to drop, so I chose to impute and encode instead. 
I used median imputation because most of the numerical data does not have a normal distribution.
## Results
Here are examples of how to embed images from your sub-folder
Item Sales Over the Years
![image](https://user-images.githubusercontent.com/62859441/181880452-240edee4-8d2a-45b5-bbd1-c8441cde69ff.png)

The plot above shows that since 1985 outlet sales have remained fairly consistent outside of one year, which was 1998.


Weight of an Item and It's MRP
![image](https://user-images.githubusercontent.com/62859441/181880483-7dccde6d-a68f-4780-a34f-5c94ebfcbe5c.png)
This plot shows the weight vs the item MSRP. It can be seen that the heavier a product is, doesn't necessarily mean it has a higher MSRP.


## Model
The final model is the decision tree regression model. I chose it because it performed the best when it came to its prediction performance. 
Applying the metrics of R^2 and RMSE it outperformed the linear regression model. 
The decision tree yielded scores of .604 (training) and .595 (testing) in R^2 vs .561 (training) and .565 (testing) for the linear regression model.
Applying RMSE metric to the two models, similar results were garnered. 
The RMSE for training and testing respectively on the decision tree model were 1082.7, and 1057.4. On the other hand the linear regression model had values of 1140.2, and 1094.9 for the training and testing sets. 
These metrics show how the decision tree model is better suited for predictive purposes as stated in the business problem. 

## Recommendations:
There could be other models out there to apply, I only explored the usage of a linear regression and a decision tree model. In the future it could be fruitful to apply a bagging or random forest model. This will allow the introduction of randomness which could or could not yield higher performance in predictive ability. 

## Limitations & Next Steps
A limitation that is consistent with or any other predictive models is the lack of data. More data can always help refine the model and increase its performance. Another limitation that I happened to find was in the correlation between the features of the data set. There was only one correlation in the data set that can be considered moderate. The correlation between Item MRP and Item Outlet Sales. This undeniably had an impact on the model. 

## For further information
For any additional questions, please contact me at dvisionstwat@gmail.com

