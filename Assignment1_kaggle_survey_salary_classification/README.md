# Assignment 1 - Background

Kaggle has hosted an open data scientist competition in 2019 titled “2019 Kaggle ML & DS Survey Challenge.” The purpose of this challenge was to *“tell a data story about a subset of the data science community represented in this survey, through a combination of both narrative text and data exploration.”* More information on the competition, data, and prizes can be found on: https://www.kaggle.com/c/kaggle-survey-2019

The original dataset (multiple_choice_responses.csv) contains the survey results provided by Kaggle. The survey results from 19717 participants are shown in 246 columns, representing survey questions. Not all questions are answered by each participant, and responses contain various data types.

In the original dataset, column Q10 “What is your current yearly compensation (approximate $USD)?” contains the ordinary categorical target variable. The original data (multiple_choice_responses.csv) has been transformed to Kaggle_Salary.csv as per the code given in KaggleSalary_DataSet.ipynb. In the dataset to be used for Assignment 1 (Kaggle_Salary.csv- File to be read in notebook for this Assignment), rows with the null values of salaries have been dropped. In addition, two columns (‘Q10_Encoded’ and ‘Q10_buckets’) has been added at the end. Column ‘Q10_buckets’(Target Variable for Assignment 1) has been obtained by combining some salary buckets in the column ‘Q10’. Column ‘Q10_Encoded’ has been obtained by label encoding the column ‘Q10_buckets’.

The purpose of this assignment is to
1) understand and explore employment in the data science community, as represented in a survey conducted by Kaggle.
2) train, validate, and tune multi-class ordinary classification problem that can classify, given a set of survey responses by a data scientist, what a survey respondent’s current yearly compensation bucket is.
