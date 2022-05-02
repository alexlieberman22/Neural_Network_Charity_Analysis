# Neural_Network_Charity_Analysis

## Overview
The purpose of this analysis was to use neural networks to create a classifier to predict whether applicants will be successful if they are funded by Alphabet Soup. The accuracy goal of the classifier was 75%.

## Results

### Data Preprocessing
- The IS_SUCCESSFUL variable was the target for the model 
- APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, etc. were all the features of the model 
- EIN and NAME were not considered either targets or features and were dropped from the dataset

### Compiling, Training, and Evaluating the Model

- For my neural network I used 3 hidden layers with neuron amounts of 100, 65, and 30 respectively and activation functions of tanh, tanh, and relu respectively. The number of neurons was decided based on the amount of inputs (~40) with the first amount being 2.5 times as many as the input and the subsequent neurons for each additional layer being much fewer each time. Tanh tended to work slightly better than relu. 
- I wasn’t able to achieve the target performance of 75%, the closest I got was 74.20% after 120 epochs 
- Some steps I took to increase the performance of the model were:
  - Dropped the columns ASK_AMT, SPECIAL_CONSIDERATIONS
  - Increased the count threshold for binning APPLICATION_TYPE
  - Added code to bin INCOME_AMT to reduce the number of unique values from 9 to 5
  - Added a hidden layer, increased the neuron amounts and changed two of the activation functions to tanh


## Summary
