# Laptop Prices Prediction using Gradient Boosted Trees (XGBoost)

This repository is about a Machine Learning to predict the price of a laptop. 

Dataset used in this repository is retrieved from [Kaggle](https://www.kaggle.com/muhammetvarl/laptop-price)

Here are the columns from the dataset:

1. Company- String -Laptop Manufacturer
2. Product -String -Brand and Model
3. TypeName -String -Type (Notebook, Ultrabook, Gaming, etc.)
4. Inches -Numeric- Screen Size
5. ScreenResolution -String- Screen Resolution
6. Cpu- String -Central Processing Unit (CPU)
7. Ram -String- Laptop RAM
8. Memory -String- Hard Disk / SSD Memory
9. GPU -String- Graphics Processing Units (GPU)
10. OpSys -String- Operating System
11. Weight -String- Laptop Weight
12. Price_euros -Numeric- Price (Euro)
___

Here is the price plotted from the dataset:
![price-plotted](https://drive.google.com/u/0/uc?id=1l0IT204NpL-E0nNbSnUD7NYsul0JldsZ&export=download)

With XGBoost, the model achieved 0.00010650141909813345 of Mean Squared Error (MSE) during training phase and 0.002709144309397954 in the testing phase. 

Here is the comparasion of the true and predicted test data:
![test-predicted-plotted](https://drive.google.com/u/0/uc?id=1-KrN0C5Xv1BF8GFJB4sV3UVupMCXvxsF&export=download)

After that, here is the comparasion of the true and denormalized predicted all data:
![all-predicted-plotted](https://drive.google.com/u/0/uc?id=143UUS0cJTZvtVA15RdAI6nzaJjnf02OU&export=download)
___

### Conclusion

A Gradient Boosted Trees (XGBoost) is a machine learning model that is better at predicting the price of a laptop from its components than a Random Forest model. It has a slightly lower MSE than random forest. If a random forest with 1250 n_estimator reaches 0.00345 MSE in the test data, then XGBoost can go lower to 0.00271 MSE. Because of that, it can be concluded that XGBoost is better than Random Forest.