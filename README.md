# Neural Network Charity Analysis

## Overview

For this project, we are helping the fictional company Alphabet Soup see whether or not a charity will be successful if they fund it. In order to accomplish this, we are going to use neural networking. By making a binary classifier, we can hopefully predict whether or not a charity will get funded before they even apply. The hope is to get the model to have 75% accuracy, or try three different models if that fails.

## Results

#### Data Preprocessing

###### What variable(s) are considered the target(s) for your model?

The variable(s) that were the targets for this model was the "IS_SUCCESSFUL" variable. The point of the model was to determine if a charity would be funded successfully, so we need to look at that.

###### What variable(s) are considered to be the features for your model?

For this model, I had every other variable be considered a feature. 43 categories is not a large amount, so I did not want to diminish the model by removing any columns or reducing it with PCA. 

###### What variable(s) are neither targets nor features, and should be removed from the input data?

There are instances in the APPLICATION_TYPE and CLASSIFICATION columns that were rare enough that it was worth compliling them into a "Other" category. Outside of that, I beleived all columns were relevant.

#### Compiling, Training, and Evaluating the Model

###### How many neurons, layers, and activation functions did you select for your neural network model, and why?

I tried three different models, all with a different amount of neurons, layers, and activation functions. Because we wanted to get the model to above 75% effeciency, played with all of the different things I could think of.

###### Were you able to achieve the target model performance?

I was not able to achieve the target model performance of 75% despite trying many kinds of models.

###### What steps did you take to try and increase model performance?

The first step I took was to use Dropout to reduce the noisy data in my model. When that didn't work, I increased the neurons of the two hidden layers from 80 and 30 to 100 and 50 respectively on my second model. For my third and final model, I added a third hidden layer of 20 neurons and changed the output function to relu.

## Summary

The overall results the four models in this project was creating something hovering around 72%-73% accuracy. While that is not the worst outcome, it is not a model that I would be thrilled recommending to companies. Instead, I would try an supervised linear regression model. Because we are ultimately trying to find a binary outcome (success or fail), linear regression might be a better tool than a neural network. 
