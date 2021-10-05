# Machine_Learing_Heart_Disease_Classification - Project Overview
This is my learning project when taking Machine Learning 0-Master course on Udemy. The goal of this project is to predict weather or not someone has heart disease based on their medical attributes via **Logestic Regression**, **KNN Classifier** and **Random Forest Classifier**  machine learning models.

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

### 6.1 Modelling and primary evaluation
* Split the data into train and test set.
* Write a function to loop through **Logisitc Regression**, **KNeighbors Classifier**, and **Random Forest Classifier**
* Compared the accuracies from three models.


![image](https://user-images.githubusercontent.com/70978272/136005548-946c3646-03a7-402f-a4c9-4b94e56301ec.png)


* Hyperparameter tuning 3 models: n_neighbors for KNN model, RandomSearchCV for Logisitic and Random Forest, and GridSearchCV for Logistic.


![image](https://user-images.githubusercontent.com/70978272/136005961-21385a71-eb2a-46a9-a196-d19cc0f12825.png)
**KNN**

### 6.2 Evaluating our tuned machine learning classifier, beyond accuracy (use Logistic as a model example)

* ROC curve and AUC score
![image](https://user-images.githubusercontent.com/70978272/136006987-f73558e2-5ff5-4da9-ad9f-4881827330d2.png)
**=from Logistic model**


* Confusion matrix

![image](https://user-images.githubusercontent.com/70978272/136007440-c338f725-3767-438c-a979-7ac63a6d980b.png)

* Classification report
* Precision
* Recall 
* F1-score

![image](https://user-images.githubusercontent.com/70978272/136007485-fb23b8ae-5d66-4557-b0f0-de1371a8dd4a.png)


### 6.3 Feature importnce (Logistic Regressor)

![image](https://user-images.githubusercontent.com/70978272/136007190-47d9057d-c7c7-412e-a2fa-51a4ad6e0c18.png)


