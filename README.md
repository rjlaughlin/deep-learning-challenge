# deep-learning-challenge

Deep Learning Challenge: Neural Network Model for Alphabet Soup

## Overview

The purpose of this analysis is to develop a neural network model that predicts whether applicants funded by charitable organization Alphabet Soup will be successful. By leveraging deep learning techniques, we aim to create a binary classifier that evaluates organizations based on various features. The primary goal is to optimize the model's performance to achieve an accuracy of at least 75%.

## Results

### Data Preprocessing

Target Variable: IS_SUCCESSFUL (Binary classification: successful or not)

Feature Variables: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT

Removed Variables: EIN and NAME (Identification fields that do not contribute to prediction accuracy.)

### Compiling, Training, and Evaluating the Model

#### Neural Network Architecture:
Input Features: Based on the preprocessed dataset.
First Hidden Layer: 16 neurons, ReLU activation function.
Second Hidden Layer: 8 neurons, ReLU activation function.
Output Layer: 1 neuron, Sigmoid activation function.


##### Model Compilation
Loss Function: binary_crossentropy
Optimizer: adam
Metrics: accuracy

##### Training and Performance:
Number of epochs: 100
Final Loss: 0.5612
Final Accuracy: 72.28%
Target Accuracy (75%) not achieved

#### Optimization Attempts
To improve the model's accuracy, several adjustments were made:

- Modified the number of neurons in hidden layers to explore different network capacities.
- Adjusted the number of hidden layers to determine if increasing depth improves accuracy.
- Changed the activation functions to alternatives like tanh and swish to test their impact.
- Tried different optimizers, but adam provided the best performance.
- Varied the number of epochs to find an optimal balance between underfitting and overfitting.

Despite these optimizations, the highest accuracy achieved was just above 72%, falling short of the 75% target.

Summary and Recommendations
The deep learning model showed some predictive ability but did not reach the target accuracy of 75%. Alternative models that might perform better include supervised learning models like SVM, Random Forest, or KNN to classify successful vs. unsuccessful companies.

