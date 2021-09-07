![header.png](https://github.com/BHashemi2021/Neural_Network_Charity_Analysis/blob/main/Resources/images/header.png)
# Neural Network Charity Analysis

## Overview of the analysis
*Alphabet Soup* is a philanthropic organization dedicated to helping organizations that protect the environment and people's well-being and unify the world.

Alphabet Soup has raised and donated over $10 billion in the past twenty years. This money has been used to invest in life-saving technologies and to organizations active in re-forestation around the world. Each donation needs to be assessed for its impact and the recipient need to be vetted by  organization's data analyst. This makes sure the organization's money is being used effectively. Unfortunately, not every donation is impactful. In some instances, an organization takes the money and will disappear. As a result the organization's president has asked their data analyst to predict which organizations are worth donating to and which are too high-risk. 

The organization's data analyst has been assigned to help create a mathematical data-driven solution that can do this accurately. Given the nature of the task, the problem is too complex for statistical and machine learning models. Instead a deep neural network needs to be designed. This model will evaluate all types of input data and produce a clear decision-making result.

Therefore, we have been tasked to help with the design and train the models using the *Python Tensorflow library*. We should employ statistics and machine learning to help test and optimize the models. We strive to create a robust *deep learning neural network algorithm* that is capable of interpreting large complex datasets. This model will help Alphabet Soup determine which organizations should receive donations.

In this undertaking we need to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. 

## Materials and Methods
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

### Data Preprocessing
* What variable(s) are considered the target(s) for your model?
The "IS_SUCCESSFUL" is the target or dependent variable which we will use to train the model.

* What variable(s) are considered to be the features for your model?
The independent variables, all the variables except the target variable, are considered the feature variables. We may remove variables like EIN and NAME that are Identification columns and are not involved in the model.


* What variable(s) are neither targets nor features, and should be removed from the input data?

The outliers, variables with unique values an th ones that are categorized as noise. Outliers can be manged be bucketing to soe extent.

### Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take to try and increase model performance?


## Summary 

Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

The model had an accuracy rate of 



xxxxxxxxxxxxxxxxxxxxx
Requirement and rubrics:

Links to images are working, and code is formatted and displayed correctly (2 pt).
Analysis (24 points)

The written analysis has the following:

Overview of the loan prediction risk analysis:

The purpose of this analysis is well defined (4 pt)
Results:

There is a bulleted list that answers all six questions (15 pt)


Summary:

There is a summary of the results (2 pt)
There is a recommendation on using a different model to solve the classification problem, and justification (3 pt)
