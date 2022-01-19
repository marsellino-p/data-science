# Predict the Price of Used Cars

This project is about a Machine Learning to predict the price of the used car. If anyone wants to sell a used car, then with this machine learning model the price of the car can be estimated.  

Dataset used in this repository is retreived from [Kaggle](https://www.kaggle.com/nehalbirla/vehicle-dataset-from-cardekho?ref=hackernoon.com&select=Car+details+v3.csv)

The following are the columns contained in the data set:
1. name
1. year
1. selling_price
1. km_driven
1. fuel
1. seller_type
1. transmission
1. owner
1. mileage
1. engine
1. max_power
1. torque
1. seat

Name and torque column were dropped because they were deemed not too important and the remaining dataset columns were sufficient for training the model. The target column is selling_price.

In this code, a random_state of 23 is used. Next, we will look for the depth of the best tree, from 1 to 25, then it is found that the tree with a depth of 21 is the best. Here is the graphic: 

![mse-graph](https://drive.google.com/u/0/uc?id=1e0GwdIdipQJVsGTsA0pwMFZho4C7ZQl2&export=download)

With Decision Tree Regression, the model achieved Mean Squared Error (MSE) of 0.00036 and R2 score of 0.94 on the test data.