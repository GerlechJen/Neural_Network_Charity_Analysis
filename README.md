# Neural Network Charity Analysis

## Overview


A non-profit philanthropic foundation Alphabet Soup dedicated to helping organizations that protect the environment, improve peoples well being, and unify the world  needs my help predicting where to make investments. The foundation has raised and donated over 10 billion dollars in the past 20 years which has been invested in life saving technologies and also used to organize reforge station groups around the world. In my current role, I analyse the impact of each donation and vet potential recipients which helps to ensure that donations are being used effectively. Unfortunately, from analysis, not all donations the company makes is impactful. Sometimes an organization takes the money and disappears.
I have been asked to design a model that will accurately predict which organizations are worth donating to and which are too high risk. I will create a mathematical data driven solution which will do this accurately. With my knowledge of machine learning and neural networks, I will design and train a deep learning neural network that will evaluate all types of input data and produce a clear decision-making result using the python TensorFlow library. From Alphabet Soup’s business team, I have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization. Using the features in the dataset I will create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.





## Results
To commence the project, I preprocessed the data in order to compile, train, and evaluate the neural network model later.


After that I compiled, trained, and evaluated the model.

Continuing, I optimized the model.

Questions to be answered 
What variable(s) are considered the target(s) for your model?
The target for the model is the IS_SUCCESSFUL column

What variable(s) are considered to be the features for your model?
The features for the mofel are the APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT        columns.

What variable(s) are neither targets nor features, and should be removed from the input data?
The 'EIN' & 'NAME' columns were expected not to have much effect on our model so were removed from the input data. 

How many neurons, layers, and activation functions did you select for your neural network model, and why?
I started my model with two layers. The first layer had 80 neurons and the second layer had 30 neurons. There was also an output layer. Each layer had an activation function. The first and second hidden layers have an activation function "relu" and the output layer is "sigmoid". 

Were you able to achieve the target model performance?
No I was not able to achieve the target model performance of 75%.

What steps did you take to try and increase model performance?

Some of the steps I took to try and make the model more accurate were:

* Removed more variables from features

* Changed the number of epochs

* Changed the number of neurons in hidden layers

* Added more hidden layers














## Summary


Increasing the number of epochs.
Binning in a different way???

----

**Completed by:** Jennifer Anno-Kusi

**Email:** jannokusi@gmail.com 
