# pro-kabaddi_hackathon
Steps for making predictions 
  - Data Selection
  - Data understanding
  - Data cleaning
  - Data transforming
  - Data visualizing
  - Model evaluation
  - Prediction
  
## Data selection
Starting with importing all the necessary libraries to be used for data extarction. Then gettign the details from url for pro kabaddi - by using a header and opening multiple urls for each team. Using beautiful soup i pared the data and created a new dataframe for getting the rows details.
I did for each team and finally i saved all in one dataframe.
## Data understanding
Now after getting the data in a table, try to understand the data- what it is related to and signifies.
It shows all team statistics - like year, number of matches, wins, loss, tie, win% and position.
It give the idea about all the team performance since the begining of the league.
## Data Cleaning
Now after knowing the data, i cleaned the data by checking for any missing values, alphabetical error etc.
I have created new columns with each team name as it wwas missing from the dataset.
## Data transforming
After cleaning, we checked the data for outliers and the type of the variables also - i found all were in object datatype.
So i changed all the columns to numerical and for categorical varaibles i created dummy varaibles to change into numerical variables.
I removed unnecesary columns from the dataset.
## Data visualizing
After creating dummy varaibles i visualized the datsaet using heatmap and pairplot to understand the vriablity of the data and the correlation between the variables.
After this i scaled the dataset and splited the dataset into x and y set.
## Model evaluation
For first step i.e model building - i imported necessary libraries
then i wanted to do this using cross validation technique hence i used it with 5 kfolds.
I used grid search CV to create a best model. I found my best model at hyperparameter value as 14. I used it in RFE and fitted the x and y in linear regression.
## Prediction
Then i predicted the model - it gave 86% accuracy which is good actually.
Next, i read the excel file for test datset to predict the winner of the pro kabaddi league 2019.
I imported it in a new dataframe. I created dummy varaibles and kept same column name as train dataset then scaled the dataset.
After this the predicted the test dataset with the model name created from train dataset.
After creating i got the winning percentage which i created in new dataframe. I added the team name to it and found the highest precentage of winning anf it is the team named as 'Haryana-steelers'.
## Haryana-steelers is predicted to win the pro kabaddi league 2019
