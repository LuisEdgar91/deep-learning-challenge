# Alphabet Soup Charity Funding Success Prediction

Alphabet Soup Charity Funding Success Prediction
Overview of the Analysis
The purpose of this analysis is to develop a binary classification model that can predict whether applicants funded by Alphabet Soup will be successful in their ventures. By analyzing a dataset of organizations that have received funding in the past, we aim to identify key features that contribute to success and build a neural network to assist Alphabet Soup in making data-driven funding decisions.

Results
Data Preprocessing
Target and Features
Target Variable:

IS_SUCCESSFUL: Indicates whether the funded organization was successful.
Feature Variables:

APPLICATION_TYPE: Type of application submitted.
AFFILIATION: Affiliated sector of industry.
CLASSIFICATION: Government organization classification.
USE_CASE: Use case for the funding.
ORGANIZATION: Type of organization.
STATUS: Active status of the organization.
INCOME_AMT: Income classification.
SPECIAL_CONSIDERATIONS: Special considerations for the application.
ASK_AMT: Funding amount requested.
Removed Variables:

EIN: Identification number for the organization.
NAME: Name of the organization.

Compiling, Training, and Evaluating the Model
Model Configuration
Input Layer:

Number of input features: Determined by the shape of X_train_scaled.
Hidden Layers:

First Hidden Layer: 80 neurons, ReLU activation function.
Second Hidden Layer: 30 neurons, ReLU activation function.
Output Layer:

1 neuron, Sigmoid activation function.

Optimization of the Model
Optimization Methods
Adjusting Input Data:

Combining rare categories into "Other".
Dropping additional columns if needed.
Modifying Neural Network Structure:

Adding more neurons to the hidden layers.
Adding more hidden layers.
Experimenting with different activation functions.
Training Adjustments:

Increasing the number of epochs.
Changing the batch size.

Summary of Results
Data Preprocessing
Target Variable: IS_SUCCESSFUL
Feature Variables: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
Removed Variables: EIN, NAME
Model Configuration
Initial Model:

2 hidden layers with 80 and 30 neurons respectively, ReLU activation.
Output layer with 1 neuron, Sigmoid activation.
Achieved an accuracy of approximately 72%.
Optimized Model:

3 hidden layers with 100, 50, and 20 neurons respectively, ReLU activation.
Output layer with 1 neuron, Sigmoid activation.
Achieved an optimized accuracy of approximately 75%.
Steps Taken to Increase Model Performance
Increased the number of neurons in the hidden layers.
Added an additional hidden layer.
Increased the number of epochs to 150.
Decreased the batch size to 16.

Recommendations for Alternative Models
To further enhance the predictive performance, alternative machine learning models such as Random Forests or Gradient Boosting could be explored. These models can handle complex interactions between features and may provide better accuracy. Additionally, hyperparameter tuning and feature engineering could be applied to refine the model further.