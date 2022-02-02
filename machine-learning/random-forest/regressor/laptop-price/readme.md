# Laptop Prices Prediction using Random Forest

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

With Random Forest, the model achieved 0.000258022146321191 of Mean Squared Error (MSE) during training phase and 0.0034489088832363604 in the testing phase. 

Here is the comparasion of the true and predicted test data:
![test-predicted-plotted](https://drive.google.com/u/0/uc?id=1BvX5HiHKmE20QWOeQrAcjtMDi8RVqdVr&export=download)

After that, here is the comparasion of the true and denormalized predicted all data:
![all-predicted-plotted](https://drive.google.com/u/0/uc?id=1jZozgb9PDmUPuipE5FZ_2hRZsJPWK3TW&export=download)
___

### Conclusion
A random forest using 1250 n_estimator is a pretty good machine learning model for predicting the price of a laptop from its components. However, this machine learning model cannot predict closely if there is a fluctuating price. This can be seen from the comparison of correct data and plotted predictions. When the price fluctuates, the model cannot predict it closely with the actual data. In conclusion, it can be a good choice model for predicting simple data.