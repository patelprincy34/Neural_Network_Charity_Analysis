# Neural_Network_Charity_Analysis
## Overview
The goal of this project is to examine and classify the success of charitable donations using deep-learning neural networks and the TensorFlow framework in Python.
For the analysis, we preprocess the data for the neural network model, then compile, train, evaluate the model and optimize the model.  

## Results
### Data Preprocessing
The identity information columns EIN and NAME have been deleted from the input data. The binary data in the IS SUCCESSFUL column indicates whether or not the charitable donation was used properly. The goal variable for our neural network is then this variable.
The characteristics for our model are the columns APPLICATION TYPE, AFFILIATION, CLASSIFICATION, USE CASE, ORGANIZATION, STATUS, INCOME AMT, SPECIAL CONSIDERATIONS.
The categorical variables were encoded, separated into training and testing datasets, and the features were standardized.
### Compiling, Training, and Evaluating the Model
We raised the hidden layers in 1 and 2 to 100 and 50 for the first model to test if the percentage would decrease if there were more neurons. In the second case, we added another hidden layer to the model to test if adding more neurons will help the model suit the data. To investigate if a more sophisticated activation might assist, we used tanh instead of relu in the third case. we couldn not get the accuracy or loss to change by much. So, we changed the "Define the model..." phase to include additional neurons in the hidden layers, tweak the activation, and add a new hidden layer.
## Summary
This model was unable to achieve the aim of 75% accuracy and did not appear to respond to modifications. With the complexities of the descion trees, Random Forest may be intricate enough to make a difference and modify the accuracy and loss.
## Resources
* Data Source: charity_data.csv
* Software: Jupyter Notebook
