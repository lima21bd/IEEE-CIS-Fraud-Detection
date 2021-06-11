## Problem Discussion:
This project is inspired from IEEE-CIS Fraud Detection Kaggle competition, where we have to solve a binary classification to predict fraudulent transaction. 

## Methodology:

  ### Data Processing:
      The training and testing dataset is separated in transaction and identity. So the dataset is merged on TransactionID for training and testing.
      There are some mismatch in training and testing features. So, the columns of test dataset is renamed to match the columns of the training data.
      There are a lots of null value. The feature containing more the 115000 null value is removed.
      The null values of the feature containing less null values will be filled with mode values.
      Memory size is reduced by changing datatype to manage this large volume of data.
      
  
  ### Feature Selection:
    Correlation is measured related to Fraud to find out the best feature.
    Features with less correlation is dropped from the dataset.

  ###   Modeling:
    XGBoost gave the state of the art accuracy. So, finetuned hyper-parameter is used to train the dataset.


  ### Result:

    XGBoost model gave the best score which is 91.15% but took too much time, around 25 mins 31 sec.

