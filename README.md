# Starbucks Capstone Project
 
 1. Introduction

    This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.

Goal:
Our goal is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type. 


Example: 
To give an example, a user could receive a discount offer buy 10 dollars get 2 off on Monday. The offer is valid for 10 days from receipt. If the customer accumulates at least 10 dollars in purchases during the validity period, the customer completes the offer.

However, there are a few things to watch out for in this data set. Customers do not opt into the offers that they receive; in other words, a user can receive an offer, never actually view the offer, and still complete the offer. For example, a user might receive the "buy 10 dollars get 2 dollars off offer", but the user never opens the offer during the 10 day validity period. The customer spends 15 dollars during those ten days. There will be an offer completion record in the data set; however, the customer was not influenced by the offer because the customer never viewed the offer.

Detailed information can be found on the following blog link :
https://medium.com/@zz42/machine-learning-tells-you-whether-a-user-will-response-to-a-starbuck-rewards-be13a882e0ca

2. Table of contents 
    1) Import LIbraries
    2) Loading Data
    3) Data Overview
    4) Data Cleaning
    5) Data Analysis
        A) Reserch into user age
            i. what is the mean of the user age
            ii. what is the distribution of user age
            iii. what is the user age distribution with different gender
            iv. what is the user distribution with different age group
        B) Reserch into user salary
            i. What is the mean of user salery
            ii. What is the salery distribution of the users with different gender
        C) Reserch into promote method
            i.What is the distribution of successful promote method
            ii. What is the distribution of promote type
            iii. What is the usage of the promote method
            iv. What is the accumulate usage of promote method with different gender
        D) Reserch into users transcript
            i. What is the mean time of purchase for users
            ii. What is the frequency distribution of users
    6) Machine learning model
            i. Data preparation
            ii. Model construction
            iii.Model modification

3. Model built based on the data set
    1) Logistic_regression_model.pkl
    2) Naive_Bayes_model_first.pkl
    3) Suport_Vector_ Machine.pkl
    
4. Evaluation of the model
    1) Logistic_regression_model.pkl
    
                    precision    recall  f1-score   support
                0       0.48      0.74      0.58     25354
                1       0.39      0.25      0.30     18854
                2       0.47      0.19      0.27     11094

            accuracy                           0.46     55302
           macro avg    0.45      0.39      0.38     55302
           
        weighted avg       0.45      0.46      0.42     55302
    2) Naive_Bayes_model_first.pkl
        
                      precision    recall  f1-score   support       
               0        0.61      0.68      0.64     25354
               1        0.49      0.41      0.44     18854
               2        1.00      1.00      1.00     11094
            accuracy                       0.65     55302
            macro avg    0.70      0.70     0.70     55302
            weighted avg 0.65      0.65     0.65     55302

    3) Suport_Vector_ Machine.pkl
 
                      precision    recall  f1-score   support
               0         0.46      1.00      0.63     25354
               1         0.00      0.00      0.00     18854
               2         0.00      0.00      0.00     11094
            accuracy                       0.46     55302
            macro avg    0.15      0.33      0.21     55302
            weighted avg 0.21      0.46      0.29     55302
    
5. Conclusion

In this project analysis of the data set is provide, meanwhile, three machine learning model was built to predict whether the costumer would response to a specific promo method. The Naive_Bayes_model have the highest accuracy of nearly 65%.
