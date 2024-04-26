# Alphabet Soup Deep Learning Model for Funding Success Prediction

## Overview of the Analysis

The purpose of this analysis is to create a binary classification model using deep learning techniques to predict if an organization funded by Alphabet Soup will be successful in their venture. The model utilizes a dataset of over 34,000 organizations that have received funding from Alphabet Soup, containing metadata about each organization.

## Results

### Data Preprocessing

- **Target variable(s) for the model:** The target variable for the model is `IS_SUCCESSFUL`.
- **Feature variable(s) for the model:** The feature variables for the model include `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, and `ASK_AMT`. 
- **Variable(s) removed from the input data:** The `EIN` and `NAME` columns were removed from the input data as they are identification columns and not useful as features or targets.

- **Feature variable** `NAME` has been brought back in the last model.

### Compiling, Training, and Evaluating the Model

- **Neurons, layers, and activation functions selected for the neural network model and rationale:** The model consists of three hidden layers with 80, 30, and 1 neurons, respectively, and ReLU activation functions. The output layer uses a sigmoid activation function for binary classification. The structure was chosen to provide a balance between complexity and the potential for overfitting, while maintaining the ability to learn complex patterns in the data.
<img width="581" alt="Screenshot 2024-04-26 100701.png" src="https://github.com/Shivabajelan/deep-learning-challenge/blob/main/images/Screenshot_2024-04-26_100701.png">
This model did not achive desired accuracy of 75%.
The accuracy achived was 72.3%. 
<img width="485" alt="Screenshot 2023-04-27 at 10 37 33 pm" src="https://github.com/Shivabajelan/deep-learning-challenge/blob/main/images/Screenshot_2024-04-26_100701.png">

In this project, we ran about 4 models. The first few models removed the EIN and NAME columns and with applying difirrent neurons and layers and binning just achived accuracy of 73%.

Model "Final-AlphabetSoupCharity_Optimisation.ipynb has the best accuracy of 78.5%.
<img width="482" alt="Screenshot 2023-04-27 at 10 37 25 pm" src="https://github.com/Shivabajelan/deep-learning-challenge/blob/main/images/Final_Screenshot_2024-04-26_103511.png">

Our **Feature variable(s) for the model:** The feature variables for the model include `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, `NAME` and `ASK_AMT`. and **Target variable(s) for the model:** The target variable for the model is `IS_SUCCESSFUL`. The model consists of three hidden layers with 14, 7, and 1 neurons, respectively, The output layer uses a sigmoid activation function for binary classification and used Relu for other layers.
<img width="595" alt="Screenshot 2023-04-27 at 10 37 20 pm" src="https://github.com/Shivabajelan/deep-learning-challenge/blob/main/images/Final_Screenshot_2024-04-26_103413.png">


- **Achievement of the target model performance:** The model did achieve the target performance of 78.85% accuracy. However, multiple attempts were made to optimize the model, including adjusting input data, modifying the structure of the neural network, and modifying the training regimen.

- **Steps taken in attempts to increase model performance:** To increase model performance, the following steps were taken:

  - Dropping additional irrelevant columns from the input data.
  - Creating more bins for rare occurrences in columns and adjusting the number of values for each bin.
  - Adding more neurons to a hidden layer.
  - Adding or removing hidden layers.
  - Using different activation functions for the hidden layers.
  - Increasing or decreasing the number of epochs in the training regimen.

### Summary

The deep learning model achieved the desired performance of 78.84% accuracy in predicting the success of Alphabet Soup-funded organizations. Several attempts were made to optimize the model through data preprocessing and neural network structure adjustments, ultimately leading to this improved performance.

