# PredictiveAnalytics: Allstate Claim Severity




This Repository is the solution of a kaggle challenge by AllState.
the link to Data Can be found here: https://www.kaggle.com/competitions/allstate-claims-severity/overview

#Step 1:
- The challenge consists of predicting the lost amount. 
- I wrote a function to read and process the data, while creating an html profiler for the data for feature engineering. 

#Step 2:
- I created an encoder to encode majority of the columns.
- I left some columns in categorical format because of the model used. 
- LightGBM has the ability to handle categorical without encoding them.

#Step 3:
- Split the training data into Training and validation.
- A testing data was provided so i left that untouched.

#Step 4:
- Set the dataset, params and train the model

#Step 5:
- predict with validation data
- calculate evalution metrics
- visualize prediction
<img width="987" alt="Validation Metrics Visualization" src="https://github.com/d0ctaa/PredictiveAnalytics/assets/99978664/8b3ea5d9-af15-48ee-b411-758b7dc22fae">

#Step 6: 
- predict with test data
- calculate evaluation metrics
- visualize precidion
<img width="1142" alt="Test Metrics Visualization" src="https://github.com/d0ctaa/PredictiveAnalytics/assets/99978664/d6635c78-f612-4ac9-b680-8414eb73d11e">

Note:  I Use Root Mean Square Error(RMSE) for my evaluation although the original competition did say they will evalute the results based on MAE
