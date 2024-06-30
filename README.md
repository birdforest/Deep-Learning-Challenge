# Deep-Learning-Challenge
Challenge 21
## Overview
- The purpose of this analysis is to create a deep learning model to predict the success of applications for funding by Alphabet Soup Charity. By analyzing historical data, the model aims to identify the significant factors that contribute to successful applications and provide a reliable prediction of future application outcomes. This will help the organization with making data-driven decisions and optimizing the funding process.
## Results

### Data Preprocessing
#### Target Variables
- 'IS_SUCCESSFUL'
#### Feature Variables
- 'APPLICATION_TYPE'
- 'AFFILIATION'
- 'CLASSIFICATION'
- 'USE_CASE'
- 'ORGANIZATION'
- 'STATUS'
- 'INCOME_AMT'
- 'SPECIAL_CONSIDERATIONS'
- 'ASK_AMT'
#### Variables Removed from Input Data:
- 'EIN': It is an identifier that is unique to each record which does not contribute to the prediction.
- 'NAME': It is an identifier that is unique to each record which does not contribute to the prediction.

### Compiling, Training, and Evaluating the Model
#### Neurons, Layers, and Activation Functions
- First Hidden Layer: 80 neurons, ReLU activation function
- Second Hidden Layer: 30 neurons, ReLU activation function
- Output Layer: 1 neuron, Sigmoid activation function
- The use of ReLU activation fuction is to handle non-linear relationships while the Sigmoid function is appropriate for binary classification tasks.
#### Target Model Performanve
- The model achieved an accuracy of approximately 72.6% on the validation data. This performance is reasonable but does not reach the ideal target of 75% accuracy.
#### Steps to Increase Model Performance
- Model 1: Increased the number of neurons in the hidden layers to ca[ture more complex patterns.
- Model 2: Added an additional hidden layer to enable the model to learn more hierarchical representations of the data.
- Model 3: Used different activation functions (tanh instead of relu) and adjusted the learning rate to improve learning stability and potentially better capture data patterns.

### Summary
- The deep learning model developed for predicting the success of Alphabet Soup Charity applications achieved an accuracy of approximately 72.6%. Even with the additionally implemented optimizations, the results provide an accuracy of approximately 72.9%, 72.7%, 72.9% for model 1, model 2, model 3, respectively. Although the optimizations do not exceed the expectation, the results still provide a solid foundation for making predictions. Improvements could be made using different model approaches such as Random Forest, Gradient Boosting, or Support Vector Machines. Random Forest help resolve overfitting issue and it provides an indication of the importance of features, which could be useful for understanding the data. Gradient Boosting focuses on correcting the errors of the previous models so it could assist with achieving high accuracy. Support Vector Machines are effective in high-dimensional spaces and they use a subset of training points in the decision function. I believe the current deep learning model provides a good starting point but with additional techniques, the performance would yield more reliable predictions for the Alphabet Soup Charity funding decisions.
