# Using regression to predict the price of wine

To collect the data we can use python to scrape prices and information about different wines. The file wines.ipynb shows how the data was collected. 

The file collects the name, price, grape-type, country of origin, and a description of the flavour. 

For predicting the price of the wine we can use different types of regression. We can convert the grape-type, flavour-description, and country of origin to a categorical by using a dictionary. 
Regression was implemented using 3 different methods: a Decision Tree Regressor, Bayesian Ridge, and a Gradient Boosting Regressor. 
The data was split into a 33% test split and mean-squared-error was used to measure the performance. This was then repeated 100 times for each method to obtain an average mean-squared-error.

On average the Bases Ridge performed the worst, with an average score of 730.7 over the 100 trials. The Decision tree and Gradient Boosting both performed around the same at 405.4 and 401.1 respectively. 

If we take a look at the predictions made (in this instance by the Gradient Boosting Regressor) then they seem for the most part reasonably accurate. We can see a sample of predicted prices compared to actual prices below; with the actual price on the left, and the predicted price on the right, for 20 samples.



Actual price | 11.99 | 9.99 | 14.99 | 55.99 | 13.99 | 8.99 | 19.99 | 12.99 | 9.99 | 9.99 | 9.99 | 16.99 | 27.99 | 17.99 | 9.99 | 9.99 | 72.99 | 11.99 | 11.99 | 9.99
--- | --- | --- | --- |--- |--- |--- |--- |--- |--- |--- |--- |--- |--- |--- |--- |--- |--- |--- |--- 
 21.06 | 17.49 |  12.49 | 36.79 | 15.99 | 10.99 | 21.06 | 17.25| 13.99 | 25.0 | 9.99 | 12.49 | 33.65 | 17.99 | 17.19 | 9.99 | 20.19 |  10.99 |  9.997 17.19 
 






# Sources 

[1] https://www.majestic.co.uk/
