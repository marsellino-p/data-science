# Classified the Suitable Drugs for Patients

This repository is about a Machine Learning to classify the suitable drug for patient. 

Dataset used in this repository is retreived from [Kaggle](https://www.kaggle.com/pablomgomez21/drugs-a-b-c-x-y-for-decision-trees)

Here is the dataset about:

Imagine that you are a medical researcher compiling data for a study. You have collected data about a set of patients, all of whom suffered from the same illness. During their course of treatment, each patient responded to one of 5 medications, Drug A, Drug B, Drug c, Drug x and y.

Part of your job is to build a model to find out which drug might be appropriate for a future patient with the same illness. The features of this dataset are Age, Sex, Blood Pressure, and the Cholesterol of the patients, and the target is the drug that each patient responded to.

It is a sample of multiclass classifier, and you can use the training part of the dataset to build a decision tree, and then use it to predict the class of a unknown patient, or to prescribe a drug to a new patient.

DATA Source: IBM

With Decision Tree, the model achieved 100% of accuracy in the test data, which mean it's a good model for the dataset. Here is the tree plotted from the model training:
![tree-plotted](https://drive.google.com/file/d/11Odfq1jgUI0CCxxsitoBlgqbUVx_5fnW/view?usp=sharing)

The confusion matrix result is:

![conf-matrix](https://drive.google.com/file/d/1iFLYUh6tAnn0zT4gy2QOMUcTUa9TGXTw/view?usp=sharing)
