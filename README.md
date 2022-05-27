# deep-learning-challenge-report
## Overview
The goal of the deep-learning-challenge is to create a predictive deep learning algorithm to determine successful funding from non-profit foundation Alphabet Soup. The task is to use the features in dataset to create binary classifiers capable of predicting success rate of organizations that are seeking funding from Alphabet Soup given data on 34,000 historically funded organizations with columns and their metadata from [charity_data.csv](https://github.com/cc-christin/deep-learning-challenge/blob/main/Resources/charity_data.csv). 

## Results

### Step 1: Preprocessing Data
'IS_SUCCESSFUL' is the target of the model, while the features are 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', 'ASK_AMT'. The columns 'EIN' and 'NAME' are neither targets nor features and were dropped. 

### Step 2: Compiling, Training, and Evaluating the Model
