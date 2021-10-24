# Neural_Network_Charity_Analysis

# Overview:

I received a CSV containing more than 34,000 organizations that have received funding over the years. Within this dataset are a number of columns that capture metadata about each organization. I used the features in the provided dataset to try and create a binary classifier that is capable of predicting whether applicants will be successful if funded.

I was asked to:

- Preprocess Data for a Neural Network Model
- Compile, Train, and Evaluate the Model
- Optimize the Model
- Submit a Written Report on the Neural Network Model

# Results:

## Data Preprocessing
- What variable(s) are considered the target(s) for your model?
    IS_SUCCESSFUL column is the target or output of the model.

- What variable(s) are considered to be the features for your model?
    All the other columns in the dataframe besides the "IS_SUCCESSFUL" column are the features. 

- What variable(s) are neither targets nor features, and should be removed from the input data?
    I removed the EIN & NAME columns as they have no effect of the target results

## Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
    I used three hidden layers. On the first layer I used 120 neurons, the second used 80, and the 3rd layer used 40. There were 40 features, and it's standard to use 2 or 3 times the number of neurons as there are features. In the end, I tried the Swish activation layer, because the folks at Google invented it and I wanted to see if it would perform better than the relu function I began with.

- Were you able to achieve the target model performance?
    I was not able to achieve the target model performance.

- What steps did you take to try and increase model performance?
    1. First I tried to remove noisy features by increasing the number of features I bucketed together. I also      removed outliers in the ASK_AMT column. 
    2. I added additional neurons and additional layers
    3. I changed the activation funtion from relu to swish

# Summary: 

I was not able to achieve the target model performance of 75%, but I got a lot of practice going through the 
steps of pre-processing data, compiling, training, evaluating the model, and exploring how to optimize the model for better performance

My recommendation to further improve accuracy, I would explore using a Sequential deep learning model with hyperparameter options. This model creates and tests many different hyperparameters and will give the reults of the best perfomning model.