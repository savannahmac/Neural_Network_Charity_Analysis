# Neural_Network_Charity_Analysis

## Overview of the analysis
The philanthropic organization, Alphabet Soup, wants to analyze the impact of each of their previous financial contributions. Their ultimate goal is to create a more effective system for vetting future orgnizations prior to donation. In order to create this system, I created a neural network model that can predict whether or not an organization is likely to be successful or unsuccessful in using the donation to make a real impact. The purpose of this step of the process is to train and test the initial model to see if it is capable of making an accurate judgment. 

## Results

# Data Preprocessing
* What variable(s) are considered the target(s) for your model?
* The target variable for this model is _succcess_. The column we'll be using as our target is 'IS_SUCCESSFUL,' which has a binary code of 1 or 0.

* What variable(s) are considered to be the features for your model?
* The features for this model are:  application type, affiliation, classification, use case, organization, income amount, and special considerations.   

* What variable(s) are neither targets nor features, and should be removed from the input data?
* In order to streamline this analysis, I removed the EIN (identification number) and the organization's name. 

# Compiling, Training, and Evaluating the Model
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
* For my model, I chose to utilize the ReLU activation function with three layers. These layers had 10, 8, and 5 nodes respectively. The ReLU activation function returns the simplest output. Since we are looking for a less-nuanced response from the model, I believed this to be the most efficient choice. Since there are 8 input features, my goal was 24 neurons. I got close, but wanted a more even distribution amongst the layers. 

Were you able to achieve the target model performance?
* I was not able to achieve the target model performance. Before and after optimization, the model was working at an accuracy of about 73%. 
![accuracy](https://user-images.githubusercontent.com/93888037/167337669-d615b32f-d176-4715-81fb-8f19f92ee89c.png)

What steps did you take to try and increase model performance?
* In order to optimize the model, I tried limiting the inputs by making stricter bins for the classification feature. Additionally, I increased the number of neurons and the number of layers. 

# Summary: 
I do not believe the model is ready for implementation at this time. More optimization must be done in order to achieve an accuracy rating between 80-85%. My recommendations are to prioritize the features and run the model with the three most important features. My instinct is that a few of the features will end up being inconsequential and may be providing too much noise to the model. Additionally, I would recommend reoptimizing the model with other activation functions to see if another function might provide better results. 
