# Titanic Passenger Survival Prediction using Gradient Boosted Trees (XGBoost)

This repository is about Machine Learning to classify whether a titanic passenger survived or not.

Dataset used in this repository is retrieved from [Kaggle](https://www.kaggle.com/c/titanic)

Here is the dataset about:

The sinking of the Titanic is one of the most infamous shipwrecks in history.

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this challenge, we ask you to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).
___
With default parameter XGBoost, the model achieved 87.2% of accuracy on the train data and 77.51% on the test data. Here is the confusion matrix result from the train data:

![conf-matrix](https://drive.google.com/u/0/uc?id=1lhgOGVD2c5tx5B8GcQF1n98h7xqCVRTL&export=download)

When I try to tune some parameters, the model achieved 97.97% of accuracy on the test data, but the accuracy on the test data is 75.12%, it's lower than default parameter XGBoost.
Here is the confusion matrix result from the train data (tuned model):

![conf-matrix-tuned](https://drive.google.com/u/0/uc?id=1-55JYbHBSS75pm6TeoYk0OYrll1Wd4Yh&export=download)
___
### Conclusion
From the result, we can conclude that the default parameter XGBoost model is better than the tuned parameter XGBoost model. In the future, we can try to re-adjusted the model parameters, for example by reducing the number of estimators, and tuned the other parameter as well.