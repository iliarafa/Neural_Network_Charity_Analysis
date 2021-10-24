# Neural_Network_Charity_Analysis

## Overview 
In this analysis we use neural networks to analyze and classify the success of charitable donations. Data preprocessing, model compilation and model optimization will be the three steps towards our objective. 

## Results 

**model features :**  APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATIONS<br><br>
**model target :** IS_SUCCESFUL<br><br>
**dropped columns :** 'EIN' and 'NAME' are neither features or targets and therefore removed from the data.

# Model Evaluation
- The initial neural network consists of two hidden layers of 80 and 30 neurons respectively. 
- Both hidden layers feature ReLu activation function and the output layer features a sigmoid activation function. 
- The initial network measured loss of 0.55 and accuracy of 0.726<br><br>

# Optimization
In the optimization that followed **three more columns were dropped:** 
- SPECIAL_CONSIDERATIONS because the value throughout the dataset is "N" <br>
- STATUS because the value throughout the dataset is 1<br>
- ASK_AMT because value visualization shows 99% of values is 5000.<br> 

#### Optimization 1
Hidden Layers: 2
Hidden Layer Neurons: 32 / 16 
Activation: Hidden Layers: Relu / Relu , Output Layer: Sigmoid
Loss: 0.58
Accuracy: 0.7075

#### Optimization 2
Hidden Layers: 3
Hidden Layer Neurons: 16 / 8 / 4 
Activation: Hidden Layers: Relu / Relu / Relu , Output Layer: Sigmoid
Loss: 0.583
Accuracy: 0.7083

#### Optimization 3
Hidden Layers: 4
Hidden Layer Neurons: 64 / 32 / 16 / 8 
Activation: Hidden Layers: Relu / Relu / Relu / Relu, Output Layer: Sigmoid
Loss: 0.587
Accuracy: 0.7080

#### Optimization 4
Hidden Layers: 2
Hidden Layer Neurons: 16 / 4  
Activation: Hidden Layers: Relu / Relu / Relu / Relu, Output Layer: Sigmoid
Loss: 0.587
Accuracy: 0.7059

# Summary
For all optimized models tested, Loss was steadily over 0.50 and accuracy stuck close to 0.71. More hidden layers and more neurons did not provide us with any significant results. On the contrary, a small number of layers featuring a small number of neurons turned out to be as accurate and slightly faster than our more complex models. This possibly signifies there is much more work to be done in reprocessing. The removal of the extra columns in optimization did not contribute to better results. Shuffling the activation functions did not result to much either. Hyperparameters appear to be irrelevant to our performance results and focus should shift to preprocessing.  Before going back to the drawing table to build new neural networks I would recommend attempting to achieve better performance with the Balanced Random Forest Classifier as we are dealing with a classification question. 


                                                                   
              

