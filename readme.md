*Prediction of diabetes based on diagnostic measurements*

**Objective:**
The objective of the dataset is to predict whether or not a patient has diabetes, based on certain diagnostic measurements. The dataset is taken from Kaggle.com.

**Dataset:**
The dataset has total 768 observations and 8 predictors. We have one target variable (binary variable) which tells us if the patient has diabetes or not.

**Procedure:**
I have designed a fully connected neural network. Input layer has 8 neurons as there are 8 inputs. The first layer has 8 neurons and third layer which is a output layer has 1 neuron. We have used ‘Relu’ as an activation function for the first layer and ‘sigmoid’ as an activation function for the output layer as we have to classify data into 2 classes.
PARAMETERS CALCULATION:
**number of input * no. of neurons + biases (1 per each neuron)
For the 1st layer: 8*8+8=72,
For 2nd layer 8*8+8=72,
For 3nd layer 8*1+1=9,
Total =153**.
I tried designing a neural network with 2 layers and it is not giving good results, I have added 3 layers to improve the accuracy. Epoch is set to 150. Optimizer is adam. Also, I have standardized the data before feeding it to neural network. 

**Conclusion:**
Following are the results after building 2 layer neural network -
The training accuracy is 75%, 
And evaluation accuracy is 62%
Which shows us that there is a overfitting.

Following are the results after building 3 layer neural network -
The training accuracy is 81%,
And evaluation accuracy is 76%
Which shows us that the accuracy is close to each other and no need to further redesign the neural network.

