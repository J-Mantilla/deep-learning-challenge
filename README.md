Report on the Neural Network Model for Alphabet Soup

Overview of the Analysis

This analysis aimed to develop a deep learning model to predict the success of charitable donations using the dataset provided by 'Alphabet Soup.' The objective was to build a neural network that accurately classifies whether a donation application will be successful based on various features. The initial model was created in the 'Starter_Code.ipynb' file using Colab and later optimized in 'AlphabetSoupCharity_Optimization.ipynb.'

Results:

Data Preprocessing:

The target variable, IS_SUCCESSFUL, indicates whether a charity application was successful.
The features used for the prediction include: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.
The columns EIN and NAME were removed from the dataset as they are neither target variables nor features relevant to the prediction.

Model Compilation, Training, and Evaluation:
Initial Model (Developed in 'Starter_Code.ipynb'):

First Hidden Layer: 80 neurons using the 'relu' activation function.
Second Hidden Layer: 30 neurons using the 'relu' activation function.
Output Layer: 1 neuron using the 'sigmoid' activation function.
The architecture was chosen to balance model complexity with computational efficiency, employing the 'relu' function in hidden layers to introduce non-linearity.
Performance: After training for 100 epochs, the model achieved a loss of 0.5983 and an accuracy of 72.80%.

Optimization Efforts (Conducted in 'AlphabetSoupCharity_Optimization.ipynb'):

First Test:

Increased the number of epochs to 200, providing the model with more opportunities to learn from the data.
This adjustment yielded a loss of 0.5712 and an accuracy of 72.72%

Second Test:

Added a third hidden layer with 100 neurons and 'relu' activation to enhance the model's ability to learn complex patterns in the data.
The model trained for 100 epochs, resulting in a loss of 0.5804 and an accuracy of 72.56%.

Third Test:

Change the two hidden layers to activiation='sigmoid' and epochs=200
The model achieved a Loss: 0.5558, Accuracy: 0.73%

Summary:

The deep learning model in this analysis initially achieved an accuracy of 72.80%. Despite multiple optimization efforts, accuracy improvements were minimal, with the highest accuracy reaching only 73%. The third optimization model proved to be the most effective, offering the highest accuracy and the lowest loss, yet none of the models exceeded a 75% predictive accuracy. All models showed very similar accuracy and loss outcomes, and the close match between test and training set accuracies indicates that overfitting is not an issue. Overall, while the model demonstrates moderate performance, it is recommended for predicting applicant success.
