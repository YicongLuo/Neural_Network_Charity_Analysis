# Neural_Network_Charity_Analysis
## Overview of the analysis
Using a neural network to help to predict if the applicants that will be funded by a Charitable organization called Alphabet Soup will be successful.
## Results

### Data Preprocessing
#### What variable(s) are considered the target(s) for your model?
- The target variable for this model was the "IS_SUCCESSFUL" column
#### What variable(s) are considered to be the features for your model?
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
-  USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested
What variable(s) are neither targets nor features, and should be removed from the input data?
[1](1.png)
- EIN and Name
### Compiling, Training, and Evaluating the Model
#### How many neurons, layers, and activation functions did you select for your neural network model, and why?
[2](2.png)
First hidden layer is 80, second hidden layer is 30.Because 40 feature columns and we use 80 neurons twice the amount of features. The first and second hidden layer have the "relu" activation function and the activation function for the output layer is "sigmoid."
#### Were you able to achieve the target model performance?
No, the result is 75%, but my model is 72.83%
[3](3.png) 
What steps did you take to try and increase model performance?
- The first test is dropping an extra feature might improve performance. The feature chosen was from the column "SPECIAL_CONSIDERATION". After re-running  after the adjustment, the model is no significant difference.
- The next test is adding more neurons to the first and second hidden layer. Specifically, 20 extra neurons were added to each, to 100 and 50 neurons to the The model is aslo no significant difference.
[4](4.png) 
- Third test is changing activation function of output layer from "sigmoid" to "tanh.The model is aslo no significant difference.
## Summary
In this neural network, we did additional optimization tests, but he predictive capability never reached above 75% accuracy. I recommand Alphabet Soup should remove more features or simply add more data to the dataset to increase accuracy. Also, we can use Random Forest Classifier. This is because random forests are a powerful and accurate model because they have a sufficient number of estimators and tree depths. Also, random forest models have faster performance than neural networks and can avoid overfitting the data.
