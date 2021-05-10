# Neural_Networks

## Overview of the loan prediction risk analysis

## Summary Analysis

The purpose of this analysis is to create a Neural Network Binary Classification capable of predicting whether applicants will be successful if funded by Alphabet Soup. In order to achieve this, a CSV file containing more than 34,000 organizations that have previously received funding from Alphabet Soup over the years is analyzed to evaluate and train data which will then serve in making a decision regarding successful applicants.

## Results

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
- Ask_AMT
- Application_Type

Unnecessary variables such as "EIN" and "NAME" were removed from the data, as they are neither targets nor features.

### Compiling, Training, and Evaluating the Model

- In order to achieve a better performance and to create more complex structures in the data, the neural network used Relu and its nonlinear activation functions. This explains the reason behind the selection of 8 neurons in the first layer, 6 in the second layer, and the output layer having a sigmoid activation function. 

![image](https://user-images.githubusercontent.com/75655852/117599558-0370fd00-b118-11eb-8ae1-6e7a11dc0512.png)

![image](https://user-images.githubusercontent.com/75655852/117599613-1f749e80-b118-11eb-9d56-eb2606750790.png)

With the optimization of the transformed data, the "STATUS" and "SPECIAL_CONSIDERATIONS" columns were removed in order to attempt to increase the model performance.The first layer of the neurons were increased from 8 to 14 and the second layer from 6 to 8. The classification count to replace values was also decreased and a callback was created to save the model's weights every 4 to 5 epochs.

![image](https://user-images.githubusercontent.com/75655852/117600659-62d00c80-b11a-11eb-909b-5317c286b4a0.png)

![image](https://user-images.githubusercontent.com/75655852/117600634-4df37900-b11a-11eb-806b-0885093d535f.png)


## Summary and recommendation 

Despite the measures taken, the target model performance of 75% accuracy was not achieved and there was little to no difference in the accuracy between the pre-optimized and the post-optimized model.

This could be explained by a number of factors such as:

- A wrong activation function may have been used
- The number of neurons used for the first and second layer needed to be changed
- The deletion of columns may have significantly altered the result (if important columns were removed)
- Different activation functions would require further testing to determine which one would be the most suitable to increase the accuracy level of the model

However, the training loss appears to have decreased from 1.02 to 0.75.

As a recommendation, a proper number of neurons as well as the right activation function need to be elaborated and chosen accurately with regards to the data in order to have a greater accuracy result.





