# Neural_Network_Charity_Analysis

Deliverable 1: Preprocessing Data for a Neural Network Model
Deliverable 2: Compile, Train, and Evaluate the Model
Deliverable 3: Optimize the Model
Deliverable 4: A Written Report on the Neural Network Model (README.md)

## Environment:
Tensorflow v. 2.4.1

## Overview of the loan prediction risk analysis:

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization.We are helping Bek, predicting whether applicants will be successful if funded by Alphabet Soup.

## Results:

* Data Preprocessing:

- What variable(s) are considered the target(s) for your model?

y = application_df.IS_SUCCESSFUL
X = application_df.drop(columns="IS_SUCCESSFUL")

Checking if target is successful or not.

- What variable(s) are considered to be the features for your model?

The "IS_SUCCESSFUL—Was the money used effectively" variable was used to see if the money funded was successful or not.

- What variable(s) are neither targets nor features, and should be removed from the input data?

EIN and NAME—Identification columns are of no use, and can be removed.

- Compiling, Training, and Evaluating the Model:

How many neurons, layers, and activation functions did you select for your neural network model, and why?

![Screen Shot 2023-01-17 at 11 26 25 PM](https://user-images.githubusercontent.com/111619125/213083996-7ac1befd-2e47-458f-8c85-f430d687366f.png)

In the optimized model, 
- layer 1 started with 110 neurons with a "relu" activation. 
- layer 2, it dropped to 80 neurons and continued with the "relu" activation. 
- layer 3, the "sigmoid" activation seemed to be the better fit with "40 neurons"
- layer 4 with "20 neurons"


Were you able to achieve the target model performance?
The target was to reach 75% accuracy but our model could just produce 72%.

What steps did you take to try and increase model performance?
-increased number of hidden layers.
-removed unnessecary columns.
-Different activation functions were used.

## Summary:
Different methods were used to reach higher accuracy for the model, however the target wasn't achieved.
Further exploration can be done using Rain forest model with more numbers of epoch as the Rain forest model has lesser outliers.

