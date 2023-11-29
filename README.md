# deep-learning-challenge

# Report on the Neural Network Model for Alphabet Soup

## Overview of the Analysis:

This document outlines the development and performance evaluation of a deep learning model for Alphabet Soup, a nonprofit foundation. The goal is to assist in selecting funding applicants with the highest likelihood of success. The dataset contains information on over 34,000 organizations, including metadata such as application type, affiliation, classification, use case, organization type, funding amount requested, and the effectiveness of the funding (IS_SUCCESSFUL).

## Results:

### Data Preprocessing:
1. What variable(s) are the target(s) for your model?
- **Target Variable(s):** IS_SUCCESSFUL
  
2. What variable(s) are the features for your model?
- **Feature Variable(s):** APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
  
3. What variable(s) should be removed from the input data because they are neither targets nor features?
- **Variable(s) to Remove:** EIN and NAME (identification columns) can be removed as they do not provide meaningful information for prediction

### Compiling, Training, and Evaluating the Model:
4. How many neurons, layers, and activation functions did you select for your neural network model, and why?
- **Neurons and Layers:**
- First hidden layer: 100 neurons, ReLU activation
- Second hidden layer: 60 neurons, ReLU activation
- Third hidden layer: 30 neurons, ReLU activation
- Output layer: 1 neuron, Sigmoid activation (for binary classification)

5. Were you able to achieve the target model performance?
- **Model Performance:** No, I was not able to achieve target model performance
- Loss: 0.5651
- Accuracy: 0.7265
  
6. What steps did you take in your attempts to increase model performance?
- **Steps Taken:**
- Adjusted the number of neurons in each hidden layer.
- Added a third layer
- Utilized ReLU activation for hidden layers and sigmoid activation for the output layer.
- Trained the model for 100 epochs.

## Summary:
This code defines a neural network with three hidden layers and one output layer. The model is trained for 100 epochs, achieving an accuracy of approximately 72.65%. Further optimizations can be explored, such as hyperparameter tuning, adjusting the number of epochs, or exploring different architectures to enhance performance.

### Recommendation for a Different Model:

While neural networks offer complexity for intricate tasks, considering simpler models like Random Forest or Gradient Boosting is advisable. These models are less prone to overfitting, easier to interpret, and may demand fewer computational resources. The choice depends on Alphabet Soup's specific needs regarding the trade-off between model complexity and interpretability.



