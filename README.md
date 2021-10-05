# Machine_Learing_Heart_Disease_Classification - Project Overview
This is my learning project when taking Machine Learning 0-Master course on Udemy. The goal of this project is to predict weather or not someone has heart disease based on their medical attributes via a Logestic Regression machine learning model.

## 1. Problem definition
Give clinical statement of a patient, can we predict weather or not they have heart disease?

## 2. Data
The original data came from Cleavland data from Machine Learning Repository. https://archive.ics.uci.edu/ml/datasets/heart+disease

There is also a version available on Kaggle: https://www.kaggle.com/ronitf/heart-disease-uci?select=heart.csv

## 3. Code and Resource Used
Python version: 3.7
Packages:  pandas, numpy, matplotlib, seaborn, sklearn

## 4. EDA
I looked into the medical medical attributes: what are they, any possible corrlation to the heart dieases. Here are some examples:

![image](https://user-images.githubusercontent.com/70978272/136003789-5c293b41-a8a0-408c-8a09-01749cf61226.png)
**Heart disease frequency according to sex**



![image](https://user-images.githubusercontent.com/70978272/136003932-53d7db73-d33a-441e-b9ae-e442928adbdd.png)
**Max heart rate and heart disease**


![image](https://user-images.githubusercontent.com/70978272/136004112-c4ed0ccf-7f40-4c00-b314-4851f18fe21a.png)
**Heart disease frequency per chest pain type**



![image](https://user-images.githubusercontent.com/70978272/136004231-fb452b85-7ecc-49e8-ad15-9c3e0815b68e.png)
**correlation matrix of medical atributes**


## 5. Data processing
There is no need to preprocess the data for this project, the data set is already processed.

## 6. Modelling and evaluation

* Set up the input and ouput shapes (the images shape, in the form of Tensors) to the model
* Set up model URL from Tensors Hub: **Keras deep learning model** : https://www.tensorflow.org/guide/keras/sequential_model
* Create TensorBoard callback and early stopping callback
* First train the model with a subset of data as a test, to check and develope the fucntion to visualize our predictions and evaluate the model
* Train the moedel with the full data set, then make predictions on the test data.
* Make custom image predictions

![image](https://user-images.githubusercontent.com/70978272/135230918-47c8c04a-f452-4c53-8146-825fec59c92d.png)


