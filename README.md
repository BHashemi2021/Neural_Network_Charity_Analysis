![header.png](https://github.com/BHashemi2021/Neural_Network_Charity_Analysis/blob/main/Resources/images/header.png)
# Neural Network Charity Analysis

## Overview of the analysis
***Alphabet Soup*** is a philanthropic organization dedicated to helping organizations that protect the environment and people's well-being and unify the world.

Alphabet Soup has raised and donated over $10 billion in the past twenty years. This money has been used to invest in life-saving technologies and to organizations active in re-forestation around the world. Each donation needs to be assessed for its impact and the recipient need to be vetted by  organization's data analyst. This makes sure the organization's money is being used effectively. Unfortunately, not every donation is impactful. In some instances, an organization takes the money and will disappear. As a result the organization's president has asked their data analyst to predict which organizations are worth donating to and which are too high-risk. 

The organization's data analyst has been assigned to help create a mathematical data-driven solution that can do this accurately. Given the nature of the task, the problem is too complex for statistical and machine learning models. Instead a deep neural network needs to be designed. This model will evaluate all types of input data and produce a clear decision-making result.

Therefore, we have been tasked to help with the design and train the models using the *Python Tensorflow library*. We should employ statistics and machine learning to help test and optimize the models. We strive to create a robust *deep learning neural network algorithm* that is capable of interpreting large complex datasets. This model will help Alphabet Soup determine which organizations should receive donations.

In this undertaking we need to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. 

## Methods
The CSV file we have received contains more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

    EIN and NAME—Identification columns
    APPLICATION_TYPE—Alphabet Soup application type
    AFFILIATION—Affiliated sector of industry
    CLASSIFICATION—Government organization classification
    USE_CASE—Use case for funding
    ORGANIZATION—Organization type
    STATUS—Active status
    INCOME_AMT—Income classification
    SPECIAL_CONSIDERATIONS—Special consideration for application
    ASK_AMT—Funding amount requested
    IS_SUCCESSFUL—Was the money used effectively
 
## Results

<span style="background-color: #FFFF00">Results</span>

### Data Preprocessing
* What variable(s) are considered the target(s) for your model?

    The "IS_SUCCESSFUL" is the target or dependent variable which we will use to train the model.

* What variable(s) are considered to be the features for your model?

    The independent variables, all the variables except the target variable, are considered the feature variables. We may remove variables like EIN     and NAME that are Identification columns and are not involved in the model.

* What variable(s) are neither targets nor features, and should be removed from the input data?

    Variables that did not classify as features or target (EIN and NAME) were removed. Moreover, variables with unique values and outliers were also    taken care of (bucketing).

### Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?

    The number of neurons and layers, especially  hidden layers, could increase the efficiency to certain extents and beyond a certain point they       would not add too much value. Accordingly, a low to moderate number of neurons were considered for the model to reduce superfluous computational processing and time (Please see below).


#### Initial results without optimization

Two hidden layers, with respectively 14 and 10 neurons, were used, . 

For the 1st and 2nd layers Relu and Sigmoid activation functions were used, respectively (Figure 1)

```ruby

# Evaluating the model using the test data
model_loss, model_accuracy = nn.evaluate(X_test_scaled,y_test,verbose=2)
print(f"Loss: {model_loss}, Accuracy: {model_accuracy}")

``` 

#### Figure 1: Results without optimization

--------------------
![Fig-1.png](https://github.com/BHashemi2021/Neural_Network_Charity_Analysis/blob/main/Resources/images/Fig-1.png)

---------------------



#### Results upon three attempts and optimization 

The model was able to reach the target value by 76% of accuracy rate after three attempts and optimization (Figure 2).


#### Figure 2: Results after three attempts and optimization

--------------------
![Fig-2.png](https://github.com/BHashemi2021/Neural_Network_Charity_Analysis/blob/main/Resources/images/Fig-2.png)

---------------------

## Summary 

Initially, the model had an accuracy rate of 73% and a loss score of 55%. Upon Optimization the model's accuracy rate improved to 76% and met the target value and the loss decreased to 48%. 

Given the low accuracy of the model, it could be applicable to preliminary screening of the applications. 

On the improvement of the model, use of a **Random Forest Classifier** might be a good option to consider as there are a noticeable number of variables or features. Moreover, addition of more data is always a great help.



