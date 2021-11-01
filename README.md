# Neural_Network_Charity_Analysis

## Overview of the loan prediction risk analysis:

The purpose of this projet is to use Machine Learning and Neural Networks to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.  The dataset contains 34,000 organizations that have been funded by Alphabet Soup. 

## Results:

### Data Preprocessing

- The IS_SUCCESSFUL column is my target variable.
- All of the variables are considered features for my model except the IS_SUCCESSFUL column and the EIN and NAME.
- The columns that I dropeed are EIN and NAME.

### Compiling, Training and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?

-  I have 2 hidden layers. The first layer has 80 neurons and the second layer has 30 neurons.  Also included is an output layer. The first and second hidden layer have the "relu" activation function and the activation function for the output layer is "sigmoid."

![image](https://user-images.githubusercontent.com/80642682/131268943-540d8616-fb86-4038-bc9e-2e45758adf14.png)


Was the model able to achieve the target model performance?

The model did not reach the target 75%. The accuracy for my model was about 62%.

![image](https://user-images.githubusercontent.com/80642682/131268983-25b868c0-a80b-416e-9e3a-f46c7ac1606e.png)


What steps did you take to try and increase model performance?

My first attempt was to remove a feature.  The feature that I removed was the 'USE_CASE' column.  The model accuracy increased to about 71%.

![image](https://user-images.githubusercontent.com/80642682/131269100-7df95df7-8f05-4457-ab69-fcad010ad64c.png)


During my second attempt I added neurons and layers.  The first layer had 100, second layer had 60, and the third layer had 20. The accuracy decreased to about 57%.
 
![image](https://user-images.githubusercontent.com/80642682/131269170-de8d2cb7-67e6-4e47-8aa8-abb8cade6926.png)

 
In my last attempt, I changed the activation of the output layer to 'tanh'. The accuracy decreased to about 47%.

![image](https://user-images.githubusercontent.com/80642682/131269230-5437af1c-a674-4e08-be4a-155158ad850d.png)


## Summary:

The highest accuracy the model scored was 71% and this is when I removed the 'USE_CASE' column.  Inorder to increase the accuracy one could remove more features or possibly add more data.  Another model that can be used to solve the classification problem is the random forest model. Random Forest is known to be accurate in the sense that is has a lot of estimators and tree depth.
