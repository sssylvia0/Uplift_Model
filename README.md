# Uplift_Model
Using different causal inference models to predict the lift value and the value lift for each customer then giving treatment.

There are three parts of the complete flow:
1. Loading the data from the MS SQL database [Predict_202312.sql]
2. Loading the data into the colab environment and there are three scripts for the colab:
  a. Preprocess
     Preprocessing the data that are used in the model.
  b. Training
     Using data from 202306 to train the data and save
  c. Prediction(Model_Nov)
     Using the data of two months before the desired month to predict the namelist of the desired month
3. Back to local
   Using local environment to write in the namelist to the db, filter the excluded people, and then make final confirmation of the namelist and the base.
   [排除條件.sql]
