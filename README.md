# deep-learning-challenge-report
## Overview
The goal of the deep-learning-challenge is to create a predictive deep learning algorithm to determine successful funding from non-profit foundation Alphabet Soup. The task is to use the features in dataset to create binary classifiers capable of predicting success rate of organizations that are seeking funding from Alphabet Soup given data on 34,000 historically funded organizations with columns and their metadata from [charity_data.csv](https://github.com/cc-christin/deep-learning-challenge/blob/main/Resources/charity_data.csv). 

## Results

### Step 1: Preprocessing Data
'IS_SUCCESSFUL' is the target of the model, while the features are 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', 'ASK_AMT'. The columns 'EIN' and 'NAME' are neither targets nor features and were dropped. 

### Step 2: Compiling, Training, and Evaluating the Model
The machine learning model used 2 hidden Relu layers with 8 and 6 neurons and a sigmoid output layer with 1 neuron as that was the conventional method utitilzed in class activities. 

The target of 75% predictive accuracy was not achived. The accuracy was 0.723 or 72.3%, slightly lower than the 75% target.

In order to improve the model. a hidden tanh layer containing 2 neurons were added, in which no improvements were made. Then the epoch was reduced in half from 100 to 50, still no noticeable improvements. Finally, a hidden Relu layer with another 8 neurons was added. The model did not have much improvement and was still approximately 72%. Overall the model improved from 0.723 to 0.724, resulting in a final accuracy of 72.4%.

The keras model fell short of reach the 75% target at only 72% and was difficult to improve. Perhaps the use of random forest classifiers would limit the undue influence of outliers and improve the model.  
