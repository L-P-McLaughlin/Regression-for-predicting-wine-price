# Using regression to predict the price of wine

To collect the data we can use python to scrape prices and information about different wines. The file wines.ipynb shows how the data was collected. 

The file collects the name, price, grape-type, country of origin, and a description of the flavour. 

For predicting the price of the wine we can use different types of regression. We can convert the grape-type, flavour-description, and country of origin to a categorical by using a dictionary. 
Regression was implemented using 3 different methods: a Decision Tree Regressor, Bayesian Ridge, and a Gradient Boosting Regressor. 
The data was split into a 33% test split and mean-squared-error was used to measure the performance. This was then repeated 100 times for each method to obtain an average mean-squared-error.

On average the Bases Ridge performed the worst, with an average score of 730.7 over the 100 trials. The Decision tree and Gradient Boosting both performed around the same at 405.4 and 401.1 respectively. 
![image](https://user-images.githubusercontent.com/60330103/222130827-f8c62e15-183f-4615-94ff-f695865de337.png)
We can see from this distribution of scores from the 100 trials that the models perform at a very similar level.

If we take a look at the predictions made (in this instance by the Gradient Boosting Regressor) then they seem for the most part reasonably accurate. We can see a sample of predicted prices compared to actual prices below; with the actual price on the left, and the predicted price on the right, for 20 samples.

|price | predicted price|
|------|---------------:|
|11.99 | 21.06 |
|9.99 | 17.49 |
|14.99 | 12.49 | 
|55.99 | 36.79 |
|13.99 | 15.99 |
|8.99 | 10.99 |
|19.99 | 21.06 |
|12.99 | 17.25 |
|9.99 | 13.99 |
|9.99 | 25.0 |
|9.99 | 9.99 |
|16.99 | 12.49 |
|27.99 | 33.65 |
|17.99 | 17.99 |
|9.99 | 17.19 |
|9.99 | 9.99 |
|72.99 | 20.19 |
|11.99 | 10.99 |
|11.99 | 9.99 |
|9.99 | 17.19 |





# Sources 

[1] https://www.majestic.co.uk/
