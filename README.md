# Predicting Bad Debt from the Lending Club dataset
This was my Capstone project for the full-time Data Science Bootcamp at BrainStation. Lending Club is a peer to peer lending platform and this data consisted of all the loans issued through the platform from 2007 to 2015. The dataset came from Kaggle.

## The Purpose
The aim of this project was to predict based on input variables of a borrower profile, whether this person will be able to pay back the loan or not.

## The Method
We decided to go with a Logistic Regression, applying a regularization of C = 0.01. We used a Standard Scaler on the data as part of preprocessing the data. The Mutual Information Score was used as a metric for assessing which variables to keep in the model and which ones to remove.

## The Data
We reduced the data from 2.26 million records with 145 variables to approximately a million records with 21 variables before using one-hot encoding for the categorical variables.

## The Result
#### Accuracy : 64%
#### Recall : 68%
#### Precision : 32%
#### F1 Score : 43.1

#### AUC Score : 0.715

The use of balanced class weights is resulting in a lot of false-positives with regards to default. Need to look into that.
NEXT UPDATE:
Use of ensembles
