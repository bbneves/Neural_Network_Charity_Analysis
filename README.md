# Neural_Network_Charity_Analysis

##Overview of the analysis: 

  With the knowledge of machine learning and neural networks, Alphabet Soup will use the features in the provided charitable dataset to help create a binary classifier that is capable of predicting whether project applicants will be successful if funded by Alphabet Soup.
  From Alphabet Soup’s business team, we've received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of characteristics that capture metadata about each organization, such as the following:
  
  - ID and NAME > Organization Identification
  - APPLICATION TYPE > Alphabet Soup application type
  - AFFILIATION > Affiliated sector of industry
  - CLASSIFICATION > Government organization classification
  - USE CASE > Use case for funding
  - ORGANIZATION TYPE
  - STATUS > Active status
  - INCOME > Income classification
  - SPECIAL CONSIDERATIONS > Special consideration for application
  - ASKING AMOUNT > Funding amount requested
  - IS SUCCESSFUL > Was the money used effectively


## Results:

## Data Preprocessing

### What variable(s) are considered the target(s) for your model?
 The target vabiable to be the results target is the successfulness of the project, whether the money was used effectvely.
 

### What variable(s) are considered to be the features for your model? And what variable(s) are neither targets nor features, and should be removed from the input data?
 We'll be using all the other variables but organaization Name and ID, because that would not be relevante for the machine learning algorithm.
 For the optimization step, we tried to remove features that had binary response which were conridered not as meaningful to the whole dataset.



Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take to try and increase model performance?
Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
