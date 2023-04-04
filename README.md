# deep-learning-challenge

## Overview
The model produced is meant to help Alphabet Soup (a non-profit foundation that funds businesses) in selecting future businesses to fund, based on whether the model thinks that the business will be successful.
The model is based on a csv supplied by Alphabet Soup that gives data based on previous businesses funded and whether they were successful.

## Results
### Data Preprocessing
- The variable that is the target for the model is *IS_SUCCESSFUL*
- The variables that are the features for the model are *APPLICATION_TYPE*, *AFFILIATION*, *CLASSIFICATION*, *USE_CASE*, *ORGANIZATION*, *STATUS*, *INCOME_AMT*, *SPECIAL_CONSIDERATIONS* and *ASK_AMT*.
- The variables that are neither are *EIN* and *NAME*.
### Compiling, Training, and Evaluating the Model
- In the first optimization of the model I used 5 hidden layers, the first of which had 25 nodes and the activation *tanh*, the second has the same activation but 20 nodes, then the third and fourth both had 15 nodes and the *selu* activation function, the fifth still used *selu* but with 10 nodes and the output layer used the @sigmoid* function.
- With this the target model performance was not reached (72.58% rather than 75%).
- In further optimizations I tried many things including dropping more columns, 'binning' more columns, less hidden layers, different activation functions and more or less nodes in the hidden layers. Although the highest performance I achieved was 72.84% test accuracy.

## Summary
The deep learning model performed very well, altough I still couldn't achieve the desired result. A supervised learning model could also solve this problem, altough it is not capable of solving as complex problems as the deep learning model, it could definitely solve this problem with something like a random forest classification.
