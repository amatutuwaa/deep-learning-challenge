# Deep Learning Challenge
#### Alphabet Soup Charity Binary Classification

## Background

Alphabet Soup, a nonprofit foundation, aims to select the applicants with the highest chances of success for funding their ventures. In this project, I use machine learning and neural networks to create a binary classifier that predicts the success of applicants funded by Alphabet Soup. A dataset containing information about more than 34,000 organizations that have received funding from Alphabet Soup has been provided. The dataset includes various columns capturing metadata about each organization, such as application type, affiliated sector of industry, government organization classification, use case for funding, organization type, and more.

## Instructions

#### Step 1: Preprocess the Data
In this step, I preprocess the dataset to prepare it for the subsequent steps of compiling, training, and evaluating the neural network model. Here are the key actions I performed:

1. Read the "charity_data.csv" file into a Pandas DataFrame.
2. Identify the target variable(s) for our model.
3. Identify the feature variable(s) for our model.
4. Drop the EIN and NAME columns.
5. Determine the number of unique values for each column.
6. For columns with more than 10 unique values, determine the number of data points for each unique value.
7. Bin "rare" categorical variables together in a new value, "Other", if needed.
8. Encode categorical variables using pd.get_dummies().
9. Split the preprocessed data into a features array, X, and a target array, y, using the train_test_split function.
10. Scale the training and testing features datasets using StandardScaler.


#### Step 2: Compile, Train, and Evaluate the Model
In this step, I design a neural network model to create a binary classifier that predicts the success of Alphabet Soup-funded organizations based on the dataset features. Here are the main actions I performed:

1. Create a neural network model using TensorFlow and Keras, considering the number of input features.
2. Create the first hidden layer with an appropriate activation function.
3. Add a second hidden layer with an appropriate activation function if necessary.
4. Create an output layer with an appropriate activation function.
5. Check the structure of the model.
6. Compile and train the model.
7. Create a callback to save the model's weights every five epochs.
8. Evaluate the model using the test data to determine the loss and accuracy.
9. Save and export the results to an HDF5 file named "AlphabetSoupCharity.h5".


#### Step 3: Optimize the Model
In this step, I optimize the model to achieve a target predictive accuracy higher than 75%. Various methods were employed for optimization, such as:

1. Adjusting the input data by dropping more or fewer columns, creating more bins for rare occurrences, or changing the number of values for each bin.
2. Adding more neurons to a hidden layer or introducing additional hidden layers.
3. Using different activation functions for the hidden layers.
4. Modifying the number of epochs in the training regimen.


#### Step 4: Write a Report on the Neural Network Model
In this step, a report was written on the performance of the deep learning model created for Alphabet Soup. The report includes the following:

1. An overview of the analysis, explaining the purpose of the analysis.
2. Results addressing the data preprocessing, including the target and feature variables, and the variables that should be removed.
3. Details on the compilation, training, and evaluation of the model, including the number of neurons, layers, and activation functions selected, and the steps taken to increase model performance.
4. A summary of the overall results of the deep learning model, along with a recommendation for a different model that could potentially solve the classification problem.



