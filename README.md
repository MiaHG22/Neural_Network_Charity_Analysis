# Neural_Network_Charity_Analysis
## Overview
The purpose of this project is to use our knowledge of machine learning and neural networks to predict whether the applicants will be successful if funded by Alphabet Soup. We will be perform the following for the analysis:

• Preprocess Data for Neural Network Model

• Compile, Train, and Evaluate the Model

• Optimize the Model

## Result
### Data Preprocessing
The variable [IS SUCCESSFUL] is the target for our model. We first removed [NAME] and [EIN] from the data because they were considered neither targets nor features. The rest we kept for features to the model. Then we used Encoder to transform all the categorial variables to numerical. 

### Compiling, Training, and Evaluating the Model
We first tried two hidden layers, ReLu to speed up the training process. We tried with 50 for the first hidden layer and 30 for the second hidden layer to test the model. Sigmoid is picked for the output layer since it's a classification model. However the result didn't reach the satisfying accuracy, only about 73%. 

<img width="681" alt="model2" src="https://user-images.githubusercontent.com/102785000/185833767-3dd39d2d-cf32-4913-a425-d6ad8c619a09.png">

Then we tried add another hidden layer and added back the variable NAME for the feature. The accuracy finaly reached to 75%. 

<img width="767" alt="3rd_try" src="https://user-images.githubusercontent.com/102785000/185833793-75ad4bb7-8667-457b-95f5-5a8dd2ccdeef.png">

## Summary
Although the accuracy met our target accuracy of 75% , the score of loss went up higher too. I think we should try the Random Forest Classifier to see if we can reach the higher result of accuacry. 

