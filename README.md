# Neural_Network_Charity_Analysis

## Overview of the Analysis
The purpose of this analysis is to develop a model that can predict if applicants that are funded by the Alphabet Soup charity will be successful.

## Results
- Data Preprocessing:
  - The "IS_SUCCESSFUL" column was the target for the model.
  - "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT" were features of our model.
  - The "EIN" and "NAME" have been removed due to being identifier information that doesn't impact the outcome.

- Compiling, Training, and Evaluating the Model
  - The model has 2 hidden layers, the 1st with 80 neurons and the 2nd with 30 layers. There is also an output layer. The hidden layers were "ReLu" activation, to help speed the process, while the output layer was "Sigmoid" activation due to the binary nature of our output.
  - The model never surpassed 75% accuracy, which isn't considered accurate enough to be effective in meeting the needs of the client.
  - In an attempt to improve the model, different activation functions were used, the number of neurons were increased, and layers were added. Unfortunately, these steps didn't improve the model. 

## Summary
The model never exceeded 75% accuracy, which is not sufficient. Instead of the model utilized here, I would recommend using a Random Forest Classifier. What we want is a binary decision of "successful" or "not successful", which a supervised machine learning model like Random Forest is perfect for.

