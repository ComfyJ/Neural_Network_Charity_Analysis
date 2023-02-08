# Neural_Network_Charity_Analysis

## Overview of the analysis: 

The purpose of our analysis is to use the features in Alphabet Soup dataset to create a binary classifier that is capable of predicting applicants success if funded by the Company.

## Results: 

Data Preprocessing:

![image](https://user-images.githubusercontent.com/104603037/190879832-617001ac-dea8-4bc6-a24f-8fb07268d2be.png)


IS_SUCCESSFUL variable(s) was considered the target(s) for my model

![image](https://user-images.githubusercontent.com/104603037/190878594-fbdb0860-71f6-4dd0-b335-c94fd29ce785.png)


The following variables were considered to be the features for my model

- APPLICATION_TYPE         
- AFFILIATION               
- CLASSIFICATION            
- USE_CASE                 
- ORGANIZATION              
- STATUS                     
- INCOME_AMT                
- SPECIAL_CONSIDERATIONS    
- ASK_AMT                    
      

Variable EIN and NAMES were neither targets nor features and they were removed from the input data

![image](https://user-images.githubusercontent.com/104603037/190878614-76cb194c-8962-486e-972b-5da40f8bc2d7.png)


Compiling, Training, and Evaluating the Model

![image](https://user-images.githubusercontent.com/104603037/190878855-5402dfb8-cd69-4f8f-8ad7-57a0616d6087.png)



I was able to select 100 neurons, 3 layers, and 2 (relu and sigmoid) activation functions for my neural network model, this is to ensure my predictions are more accurate. 


The target model performance with a predictive accuracy around 70% was achieved.

![image](https://user-images.githubusercontent.com/104603037/190879411-94ec0316-d5ca-44b2-a627-9a202d0147fe.png)

Steps taken to increase model performance
Adjusting the input data to ensure that there are no variables or outliers that are causing confusion in the model, such as:
- I dropped fewer columns.
- I created more bins for rare occurrences in columns.
- I Increased decreasing the number of values for each bin.
- I added more neurons to a hidden layer to make it 3 hidden layers.
- Adding more hidden layers.
- I used sigmoid activation functions for the hidden layers.
- I added the number of epochs to the training regimen.

![image](https://user-images.githubusercontent.com/104603037/190879442-0c212259-c930-401d-9d99-cf75ec1e7742.png)

## Summary: 

Looking at the results of our original model which achieved a predictive accuracy around 70% and the optimization model achieved around 73%.The variance in the performance of the model means we achieved a reasonable approximation of how well your model is performing in predicting whether applicants will be successful if funded by the Alphabet Soup.

My additiional recommendation is to also use the  to the random forest classifier this classification problem,because it will be able to train on the large dataset and predict values in seconds.
