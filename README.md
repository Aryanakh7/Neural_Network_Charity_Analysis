# Neural_Networks

## Overview of the loan prediction risk analysis

## Summary Analysis

The purpose of this analysis is to create a Neural Network Binary Classification that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. In order to achieve this, a CSV file which contains more than 34,000 organizations that have previously received funding from Alphabet Soup over the years is analyzed to evaluate and train data which will then serve in making a decision regarding successful applicants.

## Results

There is a bulleted list that answers all six questions (15 pt)

### Data Preprocessing 

The variable considered to be the target for the model is "IS_SUCCESSFUL".

The features of the model Include:

- Affiliation
- Classification
- Use_Case
- Organization
- Income_AMT
- Special_Considerations
- Status
- Ask_Amt
- Application_Type

Unnecessary variables such as "EIN" and "NAME" were removed from the data, as they are neither targets nor features.

### Compiling, Training, and Evaluating the Model

- In order to achieve bette performance and to create more complex structures in the data, the Neural Network used Relu and its nonlinear activation functions. This explains the reason behind the selection of 8 neurons in the first layer, 6 in the second layer, and the output layer having a sigmoid activation function. 

![image](https://user-images.githubusercontent.com/75655852/117599558-0370fd00-b118-11eb-8ae1-6e7a11dc0512.png)

![image](https://user-images.githubusercontent.com/75655852/117599613-1f749e80-b118-11eb-9d56-eb2606750790.png)

With the optimization of the transformed data, the "STATUS" and "SPECIAL_CONSIDERATIONS" columns were removed in order to attempt to increase the model performance.

Were you able to achieve the target model performance?
What steps did you take to try and increase model performance?

## Summary and recommendation 

There is a summary of the results (2 pt)
There is a recommendation on using a different model to solve the classification problem, and justification (3 pt)




