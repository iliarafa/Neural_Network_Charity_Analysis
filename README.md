# Neural_Network_Charity_Analysis

## Overview 
In this analysis we use neural networks to analyze and classify the success of charitable donations. Data preprocessing, model compilation and model optimization will be the three steps towards our objective. 

## Results 

model features : APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
model target : IS_SUCCESFUL 
columns 'EIN' and 'NAME' are neither features or targets and therefore removed from the data.

# Model compilation, evaluation and optimization
- The initial neural network consists of two hidden layers of 80 and 30 neurons respectively. 
- Both hidden layers feature ReLu activation function and the output layer features a sigmoid activation function. 
- The initial network measured loss of 0.55 and accuracy of 0.726
- 
