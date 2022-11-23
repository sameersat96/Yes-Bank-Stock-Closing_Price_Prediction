# Yes-Bank-Stock-Closing_Price_Prediction
Yes Bank Limited is an Indian private sector bank headquartered in Mumbai, India and was founded by Rana Kapoor and Ashok Kapur in 2004. It offers wide range of differentiated products for corporate and retail customers through retail banking and asset management services. On 5 March 2020, in an attempt to avoid the collapse of the bank, which had an excessive amount of bad loans, the Reserve Bank of India (RBI) took control of it.

![image](https://user-images.githubusercontent.com/95841292/202706607-372b1391-c041-40a0-8528-c51be84f60c9.png)


# 📋 Problem statement

Yes Bank is a well-known bank in the Indian financial domain. Since 2018, it has been in the news because of the fraud case involving Rana Kapoor. Owing to this fact, it was interesting to see how that impacted the stock prices of the company and whether Time series models or any other predictive models can do justice to such situations. This dataset has monthly stock prices of the bank since its inception and includes closing, starting, highest, and lowest stock prices of every month. The main objective is to predict the stock’s closing price of the month.



# 📋 Visualizations

# 1) stock price over time 

![newplot (1)](https://user-images.githubusercontent.com/95841292/202969391-4d329a04-d847-43f8-97cf-aff966241001.png)

# 2) correlation 

![image](https://user-images.githubusercontent.com/95841292/202969499-52f1114e-00b6-4478-a459-651dbb0aa5fa.png)



# 📋 Model used-

# Ridge regression

![image](https://user-images.githubusercontent.com/95841292/202969659-64c6876a-615d-45d5-b644-11e15393fa11.png)


# Lasso regression

![image](https://user-images.githubusercontent.com/95841292/202969694-4a90d25c-d798-424e-8b37-4d80ab684b7d.png)


# KNN regressor

![image](https://user-images.githubusercontent.com/95841292/202969567-e3c30afe-9701-4681-b0d3-501f38873480.png)


We performed Linear regression setting high, low and open as independent variables. Divided the dataset into training and testing datasets. We transformed the data using MinMax scaler which transforms each feature in a given range. We predicted the closing price of the test data using the Linear regression model we have trained.

Also, to check how other models perform, we performed Lasso regression and Ridge regression, both with alpha 0.1 and maximum iterations of 3000 with the same datasets used for training Linear regression. We performed Cross validation and got the best fit alpha value. We predicted the closing price of the test data using the Lasso regression model and ridge regression respectively.

Moving forward, we calculated the various performance metrics like MAE, MAPE, MSE, RMSE, r2 scores for all the three models. Finally, we plotted the actual values vs predicted values of the closing price for all of them. Linear Regression has given the best results with lowest MAE, MSE, RMSE and MAPE scores. Ridge regression shrunk the parameters to reduce complexity and multicollinearity, but ended up affecting the evaluation metrics. Lasso regression did feature selection and ended up giving up worse results than ridge which again reflects the fact that each feature is important.

# 📋 model performance

![ss](https://user-images.githubusercontent.com/95841292/202707156-bfc3d550-c9b9-4827-8740-11da79258091.PNG)


# 📋 Conclusion
-  In EDA part we observed that
1.  There is increase in trend of Yes Bank's stock's Close,Open,High,Low price till 2018 an then sudden decrease.
2.  We observed that open vs close price graph concluded that after 2018 yes bank's stock hitted drastically.
3.  Target variable(dependent variable) strongly dependent on independent variables
4.  We get maximum accuracy of 99%
5.  Linear regression and Ridge regression get almost same R squared valueWhereas Lasso model shows lowest R squared value and high MSE,RMSE,MAE,MAPE
6.  Ridge regression shrunk the parameters to reduce complexity and multicollinearity but ended up affecting the evaluation metrics.


# 📜 Credits

Sameer Satpute | Data Scientist | Machine Learning Engineer | Deep Learning enthusiast

Special thanks AlmaBetter

Contact me for Data Science Project Collaborations

[![image](https://user-images.githubusercontent.com/95841292/202914376-d5a83f3d-110a-4476-896e-1da078b185dc.png)](https://www.linkedin.com/in/sameersatpute/)
[![image](https://user-images.githubusercontent.com/95841292/202914715-787f6ae3-d9f6-491c-9cae-c717131ddebd.png)](https://github.com/sameersat96)
[![image](https://user-images.githubusercontent.com/95841292/202914883-bce71634-6c2b-4305-8020-4b240cb76e41.png)](https://medium.com/@sameersatpute)
![image](https://user-images.githubusercontent.com/95841292/202914940-5d5eba71-e45d-4e95-8dfe-65e45d255aec.png)




# 📚 References

1. https://trendlyne.com/research-reports/stock/1535/YESBANK/yes-bank-ltd/
2. https://www.ijraset.com/research-paper/stock-market-prediction-using-ml
