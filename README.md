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
