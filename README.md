# Overview
The purpose of this analysis was to utilize machine learning and deep neural networks to predict whether different organizations will be successful if funded. A dataset containing information about previously funded applications was used to train the nueral network, with information about each organization including application type, affiliation, classification, use case, organization type, active status, income classification, special considerations and amount requested. First the model was created and run, then duplicated and altered in an attempt to improve the accuracy of the model.

# Results
## Data Processing
*The variable that is considered a target for the model if the organization will be successful
*Variables that are considered features are application type, affiliation, classification, use case, organization type, active status, income classification, special considerations and amount requested
*Variables that are neither targets nor features are EIN and name of organization

## Compiling, Training and Evaluating
*Initially two layers were used, the first had 80 nuerons and the second had 30. The input layer and both hidden layers used Relu activation functions and the output used a sigmoid activation function. 
*The first model achieved an accuracy score of 72.6%, which is short of the target accuracy of 75%
*A variety of steps were taken to increase model performance. An additional hidden layer was added, and the number of neurons was increased in each layer to 120, 90 and 60 respectively. The activation function for the output layer was changed from sigmoid to Relu and the number of epochs was increased to 150. 
![codescreenshot](https://github.com/mayamtims/Neural_Network_Charity_Analysis/blob/main/screenshot.png)

# Summary 
Overall, after the deep learning model was ran there was a loss of .61 and an accuracy score of .72. This means that the model correctly categorized whether an organization would be successful or not if provided funding 72% of the time. The target accuracy score was 75%, which was not met. It is reccommended that a Random forest model be created and run instead to see if a higher accuracy score can be achieved. With enough estimators and number of trees this model could preform similarly to a deep neural network, while requiring less code and a shorter run time.   