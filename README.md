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



### Compiling, Training, and Evaluating the Model

 For the main deep learning (DL) model, we did:
  - Neurons: 80, 30, 1
  - Activation Functions: relu, relu, sigmoid
  - Epoch: 100

<img width="622" alt="AlphabetDeepLearning" src="https://user-images.githubusercontent.com/103459820/187284664-645b65d7-f5f8-450b-aa04-b222b1d86f3d.png">

 For the First Optimization DL model:
  - Neurons: 52, 26, 1
  - Activation Functions: relu, relu, sigmoid
  - Epoch: 100

<img width="633" alt="Opt_1" src="https://user-images.githubusercontent.com/103459820/187284939-bfedfc99-9875-4b47-814d-f8bb5be46301.png">

 For the Second Optimization DL model:
  - Neurons: 52, 26, 1
  - Activation Functions: tanh, relu, sigmoid
  - Epoch: 120
 
<img width="636" alt="Opt_2" src="https://user-images.githubusercontent.com/103459820/187285103-f837c44b-c57c-407d-88ad-9a6c85d81903.png">

 For the Third Optimization DL model:
  - Neurons: 60, 30, 1
  - Activation Functions: tanh, relu, softmax
  - Epoch: 150

<img width="631" alt="Opt_3" src="https://user-images.githubusercontent.com/103459820/187285299-f44f3027-7648-4f70-85f3-451cfcde2f01.png">

We weren't able to achieve a performance above accuracy of 0.75.
We attempt modifing the data input and the algorithm attributes in many diffent possibilities. We didn't get better results, however, we can use this attempts to narrow down to better combinations in order to optimize in the next attempts.

Summary: We reccomend furthering investigation on attributes, and including all the data information from the main DL model. Then, utilize the algorithm attributes that kept at least similar accuracy as the mais one as new parameters for other attempts.
