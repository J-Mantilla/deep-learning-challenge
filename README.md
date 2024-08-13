Overview
The purpose of this analysis was to develop a deep learning model to predict the success of charitable donations using the dataset provided by 'Alphabet Soup.' The goal was to create a neural network that accurately classifies whether an application will be successful based on various features such as organization type, income amount, asking amount, and affiliated industry.

The analysis was carried out in two stages:

Model Development:

The initial model was developed using the 'Starter_Code.ipynb' file in Google Colab. This involved preprocessing the data, including handling categorical variables, splitting the dataset into training and testing sets, and scaling the features.
A Sequential neural network model was created and trained with different input dimensions, activation functions, and nodes. The model was compiled and evaluated for its performance.
Model Optimization:

The model was further refined in the 'AlphabetSoupCharity_Optimization.ipynb' file to achieve a predictive accuracy greater than 75%. Optimization involved adjusting the model architecture and training parameters.

Steps
Step 1: Preprocess the Data

Upload & Read Data:
Upload charity_data.csv to Google Colab and read it into a Pandas DataFrame.
Identify & Clean Variables:
Determine target and feature variables, then drop EIN and NAME columns.
Analyze & Encode:
Identify unique values, combine rare categories into "Other," and use pd.get_dummies() for encoding.
Split & Scale:
Create feature (X) and target (y) arrays, split into training and testing sets, then scale features with StandardScaler.
Step 2: Compile, Train, and Evaluate the Model

Design & Build:
Create a neural network with TensorFlow/Keras, define layers and activation functions.
Compile & Train:
Add and compile layers, include a callback to save weights every five epochs, and train the model.
Evaluate & Save:
Evaluate the model's performance, then save it to AlphabetSoupCharity.h5.
Step 3: Optimize the Model

Setup:
Create AlphabetSoupCharity_Optimization.ipynb.
Preprocess:
Repeat preprocessing with any necessary adjustments.
Optimize & Save:
Refine the model to exceed 75% accuracy by adjusting parameters, then save to AlphabetSoupCharity_Optimization.h5.
Step 4: Write a Report

Overview:
Explain the analysis purpose.
Results:
Detail target/features, removed columns, model architecture, and performance.
Summary:
Summarize findings and suggest alternative models.
Step 5: Copy Files Into Your Repository

Download & Move:
Download notebooks, move them to your Deep Learning Challenge directory.
Push Files:
Push the files to GitHub for final submission.
