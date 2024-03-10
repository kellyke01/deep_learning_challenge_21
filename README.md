Step 1: Preprocess the data:
  Read the charity_data csv into a Pandas Dataframe and identify what variables are the target of the model and what variables are the features for the model.
  Drop both EIN and NAME columns. Count the unique values for each column.
  For columns with more than 10 unique values, determine the data points for each value.
  Then use the number of datapoints for each value to pick a cutoff point to bin rare categorical variables together in a new value of 'Other'. Check to make sure it was successful.
  use pd.get_dummies to encode those variables.
  split to preprocessed data into a features array (x) and a target array (y). use the train_test_split function to split the data into training and testing datasets.

Step 2: Compile, Train and Evaluare the Model;
  Using TensorFlow, design a Deep Learning Model to create a binary classification model that can predict if an Alphabet Soup- funded organization will be successful based on the features in the dataset.
  Assign the number of input features and nodes for each layer using TensorFlow and Keras.
  Create two hidden layers and an output layer with their appropriate activation functions.
  Check the structure of the model and compile and train it. 
  Then create a callback that saves the model's weights every 5 epochs.
  Evaluate that model using test data to determine loss and accuracy.
  Export your results to HDF5.

Step 3: Optimize the Model
  In a new notebook use TensorFlow to optimize your mode lto achieve a target predictive accuracy higher than 75%.
  Adjust the input data to ensure that no variables or outliers are causing confusion in the model, such as:
    Dropping more or fewer columns.
    Creating more bins for rare occurrences in columns.
    Increasing or decreasing the number of values for each bin.
    Add more neurons to a hidden layer.
    Add more hidden layers.
    Use different activation functions for the hidden layers.
    Add or reduce the number of epochs to the training regimen.

Step 4: Write a Report on the Neaural Network Model
Data Preprocessing

What variable(s) are the target(s) for your model?
    application type, affiliation, classification, use case, organization, income amount and ask amount.
What variable(s) are the features for your model? 
    if it was successful is my target variable.
What variable(s) should be removed from the input data because they are neither targets nor features? EIN, Status and Special Considerations.

Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why? 
    100, 30 and 10.
Were you able to achieve the target model performance? 
    Yes, I got a 79% accuracy.
What steps did you take in your attempts to increase model performance? 
    I removed columns that did not benefit me, I also replaced counts lower than certain amounts (1000, 500, etc.) so small data would be grouped together for a better outcome.

Summary: Summarize the overall results of the deep learning model. 
Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
    I used Random Forest Classifier on the dataset to maybe solve the classification problem, and it did get an accuracy of higher than 75%,
    but it didn't get higher than my original preprocessed work did.




    
