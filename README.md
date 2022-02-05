# Neural_Network_Charity_Analysis

## Overview
The purpose of this project was to help a non-profit foundation predict which organizations are worth donating to and which are too high risk. To accomplish this task, the impact of each of the 34,000 previous recipients was analyzed.  

Using Python's Tensor-flow library, I designed, trained, and evaluated a deep learning neuro network. The goal was to create a model that evaluates many categories of input data to accurately predict the most cost-effective use of money for future donations.

This was accomplished in three steps
 1. Preprocessed the data for the neural network model.
 2. Compiled, trained, and evaluated the model.
 3. Optimized the model.

## Results

Data Preprocessing
- The target variable for my model is: Is Successful
- The feature variables are: Application Type, Affiliation, Classification, Use Case, Organization, Status, Income Amount, Special considerations, Ask Amount 
- The original dataset had two variables that were neither targets nor features, so were removed from the model:  EIN and Name


Compiling, Training, and Evaluating the Model
- My final model had three hidden layers, with 80, 50, and 40 nodes respectively. All three hidden layers used the tanh activation method. It also had an output layer that used the sigmoid activation method.  
- Unfortunately, I was not able to achieve the goal accuracy performance of 75%. The accuracy level only increased 0.14% in between the original and final models. 

Optimizing the Model
- I took the following steps in an effort to improve the level of accuracy: 
 1. Increased the number of nodes to the second layer.
 2. Added a third hidden layer.
 3. Changed the activation method from 'relu' to 'tanh'.

The accuracy score from each of the four models are below: 

![accuracy_charts](https://user-images.githubusercontent.com/90162669/152655892-dea0b7d0-68fa-4510-a37a-534d70336c8a.png)

The following is the summary information from the final model: 

![Model_c_summary](https://user-images.githubusercontent.com/90162669/152656493-10b8ebd5-90cf-45ca-bfde-5dff2e6b44f0.png)


## Summary
The goal was to achieve an accuracy score of at least 75% and my model fell short of that goal with an final accuracy level of 73%. I recommend looking at other model types such as Random Forest Classifier or SMOTEENN to determine if the accuracy level would be greater. 
