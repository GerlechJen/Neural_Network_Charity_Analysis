# Neural Network Charity Analysis

## Overview


A non-profit philanthropic foundation Alphabet Soup dedicated to helping organizations that protect the environment, improve peoples well being, and unify the world  needs my help predicting where to make investments. The foundation has raised and donated over 10 billion dollars in the past 20 years which has been invested in life saving technologies and also used to organize reforge station groups around the world. In my current role, I analyse the impact of each donation and vet potential recipients which helps to ensure that donations are being used effectively. Unfortunately, from analysis, not all donations the company makes is impactful. Sometimes an organization takes the money and disappears.

I have been asked to design a model that will accurately predict which organizations are worth donating to and which are too high risk. I will create a mathematical data driven solution which will do this accurately. With my knowledge of machine learning and neural networks, I will design and train a deep learning neural network that will evaluate all types of input data and produce a clear decision-making result using the python TensorFlow library. From Alphabet Soup’s business team, I have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization. Using the features in the dataset I will create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results
To commence the project, I preprocessed the data in order to compile, train, and evaluate the neural network model later. I encoded the categorical variables using one-hot encoding and standardized numerical variables using Scikit-Learn’s StandardScaler class. After preprocessing, the dataframe looked like this:

![image1](https://github.com/GerlechJen/Neural_Network_Charity_Analysis/blob/main/IMAGES/image2.png)

Afterwards using TensorFlow, I designed a neural network to create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the dataset. The number of input features was 43. I used two layers. The first layer had 80 neurons and the second layer had 30 neurons. There was also an output layer. Each layer had an activation function. The first and second hidden layers have an activation function "relu" and the output layer is "sigmoid". The image below shows the structure of the model. 

![image](https://github.com/GerlechJen/Neural_Network_Charity_Analysis/blob/main/IMAGES/model_structure.png)

I then compiled, trained, and evaluated the binary classification model to calculate the model’s loss and accuracy. The results are shown in the below image:

![image4](https://github.com/GerlechJen/Neural_Network_Charity_Analysis/blob/main/IMAGES/model_performance.png)

As seen from the image above, the accuracy of the model was 72.9% . My goal was to obtain a predictive accuracy higher than 75%. So I tried optimizing the model in three different scenarios. In my first attempt I had a similar accuracy of 72.9%. My second attempt produced an accuracy of 72.7% and third attempt an accuracy of 71.3%.

### Questions to be answered 

- What variable(s) are considered the target(s) for your model?

The target for the model is the IS_SUCCESSFUL column

- What variable(s) are considered to be the features for your model?

The features for the model are the APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT        columns.

- What variable(s) are neither targets nor features, and should be removed from the input data?

The 'EIN' & 'NAME' columns were expected not to have much effect on our model so were removed from the input data. 

- How many neurons, layers, and activation functions did you select for your neural network model, and why?

I started my model with two layers. The first layer had 80 neurons and the second layer had 30 neurons. There was also an output layer. Each layer had an activation function. The first and second hidden layers have an activation function "relu" and the output layer is "sigmoid". 

- Were you able to achieve the target model performance?

No I was not able to achieve the target model performance of above 75%.

- What steps did you take to try and increase model performance?

Some of the steps I took to try and make the model more accurate were:

1. Removing more variables from features.

2. Binning the INCOME_AMT column.

3. Decreasing the number of values for the APPLICATION_TYPE bin.

4. Changing the number of epochs.

5. Changing the number of neurons in hidden layers.

6. Adding more hidden layers.

7. Changing the activation function of some hidden layers to tanh.


## Summary
The model's accuracy was always approximately 73%. In one instance it was just 71.3%. The goal of a predictive accuracy above 75% could not be attained after various attempts were made. If there was more data the accuracy could have probably been increased. 

My recommendation is to use the RandomForest Classifier model. This model can handle binary features, categorical features, and numerical features. It requires very little pre-processing and the data does not need to be rescaled or transformed. The RandomForest model also produces higher level of accuracy in predicting outcomes. 

----

**Completed by:** Jennifer Anno-Kusi

**Email:** jannokusi@gmail.com 
