Alphabet Soup Charity Deep Learning Challenge

Overview
The purpose of this analysis was to develop a deep learning model to predict the success of charitable donations using the dataset provided by 'Alphabet Soup.' The goal was to create a neural network that accurately classifies whether an application will be successful based on various features such as organization type, income amount, asking amount, and affiliated industry.

The analysis was carried out in two stages:

Model Development:

The initial model was developed using the 'Starter_Code.ipynb' file in Google Colab. This involved preprocessing the data, including handling categorical variables, splitting the dataset into training and testing sets, and scaling the features.
A Sequential neural network model was created and trained with different input dimensions, activation functions, and nodes. The model was compiled and evaluated for its performance.
Model Optimization:

The model was further refined in the 'AlphabetSoupCharity_Optimization.ipynb' file to achieve a predictive accuracy greater than 75%. Optimization involved adjusting the model architecture and training parameters.
The preprocessing steps included establishing cutoffs for features with many unique values, converting categorical data to numeric format, and scaling the data. The final model was optimized to enhance its performance and accuracy in predicting the success of charitable applications.

Step 1: Preprocess the Data
Upload and Read Data

Upload the charity_data.csv file to Google Colab.
Read the CSV into a Pandas DataFrame.
Identify Variables

Determine which variable(s) will be your target(s) and which will be your feature(s).
Drop the EIN and NAME columns.
Analyze Unique Values

Determine the number of unique values for each column.
For columns with more than 10 unique values, count data points for each unique value.
Combine rare categorical variables into an "Other" category as needed.
Encode Categorical Variables

Use pd.get_dummies() to convert categorical variables into numerical format.
Split Data

Create feature (X) and target (y) arrays.
Use train_test_split to divide the data into training and testing sets.
Scale Features

Instantiate a StandardScaler.
Fit the scaler on the training data and transform both the training and testing features.
Step 2: Compile, Train, and Evaluate the Model
Design Neural Network

Determine the number of inputs based on features.
Create a neural network using TensorFlow and Keras with appropriate layers and activation functions.
Build and Compile the Model

Add the first hidden layer with an activation function.
Optionally, add a second hidden layer.
Create an output layer with a suitable activation function.
Compile the model.
Train the Model

Include a callback to save the model's weights every five epochs.
Train the model on the training data.
Evaluate the Model

Assess the model’s performance on the test data, calculating loss and accuracy.
Save the Model

Export the model to an HDF5 file named AlphabetSoupCharity.h5.
Step 3: Optimize the Model
Create a New Colab File

Name it AlphabetSoupCharity_Optimization.ipynb.
Import Dependencies and Preprocess Data

Repeat the preprocessing steps from Step 1 with any adjustments for optimization.
Optimize Neural Network

Adjust the model by adding or reducing neurons, hidden layers, changing activation functions, or modifying epochs to achieve higher than 75% accuracy.
Save the Optimized Model

Export the optimized model to an HDF5 file named AlphabetSoupCharity_Optimization.h5.
Step 4: Write a Report on the Neural Network Model
Overview

Explain the purpose of the analysis.
Results

Data Preprocessing:
Identify target and feature variables.
Specify any columns removed from the dataset.
Model Details:
Describe the architecture: neurons, layers, and activation functions.
Report on whether the target accuracy was achieved and the steps taken to improve performance.
Summary

Summarize the results.
Include recommendations for alternative models and improvements.
Step 5: Copy Files Into Your Repository
Download Files

Download your Colab notebooks to your local machine.
Move and Push Files

Move the files into your Deep Learning Challenge directory.
Push the files to GitHub for final submission.
