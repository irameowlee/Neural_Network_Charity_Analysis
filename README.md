# Module 19 Challenge
### Neural Networks and Deep Learning Models
 
## Overview of the analysis: 
Alphabet soup wants Bek to analyze which charity groups are worth donating to and which groups are high-risk.
Bek wants to design and train a deep learning neural network that evaluates all types of input data and produce clear decision making results.
We use python tensorflow library and created a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results

### Data Preprocessing
![](/Resources/df.png)

- What variable(s) are considered the target(s) for your model? : IS_SUCCESFUL column
- What variable(s) are considered to be the features for your model? : APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
- What variable(s) are neither targets nor features, and should be removed from the input data? : EIN & NAME

### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
: 80 neurons for first layer, 30 neurons for second layer. All of the hidden layers used the relu activation function to identify nonlinear characteristics from the input values. In the output layer, used the same parameters from our basic neural network including the sigmoid activation function. The sigmoid activation function helps us predict the probability.
- Were you able to achieve the target model performance? 
: No. Target predictive accuracy should be higher than 75%.
- What steps did you take to try and increase model performance?
: Dropping more or fewer columns, added more neurons to a hidden layer, Added more hidden layers, used different activation functions for the hidden layers, changed number of epochs to the training regimen.

## Summary 
![](/Resources/optimized.png)
I was able to increase the accuracy score from 57% to 70% by increasing the epochs to the training regimen.
Dropping more columns and adding more hidden layers and increasing neurons did not improve the accuracy of the model. Although we were not able to reach the target predictive accuracy, gaining more relevant data for the model would achieve higher accuracy. 