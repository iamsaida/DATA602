## Introduction

The main motivation behind selecting this data set is that, usually the Department of Building and Safety issues permit based on the various types of requirements for the buildings. 

These include construction, remodeling etc. These permits are classified into mechanical, electrical etc. for the scope of this project classification of these permits into either automatic e permits or should the application require manual intervention must be decided based on the data provided by the contractor. 

This automates the process of providing a permit to a contractor based on the  model trained. It minimizes the latency for the constructor to begin his intended project. It accelerates the construction process and increases the revenues for the state

Abstract

The dataset consisting of applicant information regarding the permit, after a deep observation of the details, his/her relationship and past experience is explored to classify whether he has to get an e-permit or does It need to be reviewed by the building and safety authority. For the e permit is confirmed by a 'No Plan Check' and if there is a verification, it returns to be as 'Plan Check'. A classification is done based on this category and a preliminary look into the various attributes are done including feature engineering. Exploratory data analysis on the data to visualize the data is done. Finally, the data is trained and tested to fit various models to form a generalized model which could classify the e-permit or a further review by the authority. Classification accuracy is calculated in the end .

Exploratory Data Analysis

Importing the required for data exploratory analysis
Reading the data using Pandas CSV
Displaying the dataset
Having a clear over the columns and first 5 rows
Finding the datatypes of the columns using info() function¶
Finding the max, min and quartiles of the columns using describe function
Plotting all the numberical columns columns using matplotlip function
Determining the correlation among the columns 
Plotting the correlation using seaborn heatmap
A scatter plot to see the distribution of each column with respect to other columns¶
Selected the target variable as 'Permit Category' and we do the analysis on precticting this column
Plotting the value cpunts of the target variable
A bar plot showing the Plan Checks and No plan checks of target variable


Data Cleaning and Modeling

Creating dummies for the target variable
Displaying the dataset after replying target variable with dummies¶
Filling the missing values with most frequent value
Verifying that there are no missing values in any column of the dataset
Splitting the train and test data¶
Performing Logistic Regression on the Dataset
Creating the processing pipeline and modeling pipeline
Fitting the model with train data and finding the results
Using GridSearch, finding the validation score and test score of Logistic Regression
Using another classifer to cross validate and find the best fit model
Using GridSearch, finding the validation score and test score of Decision Tree classifier

Results

Total number of training samples: 1,100,377  
Total number of testing samples: 275,095  

Logistic regression  
Logistic regression using Grid search  
Permit  : Precision (0.88) , Recall ( 0.42), F1 score (0.56)  
No permit : Precision (0.77), Recall (0.96), F1 score (0.86)

Validation score: 77.23%, Test score: 77.04% 
Decision trees:  Validation score: 87.61%  Test score: 87.96%

Conclusion

The test score value for decision tree classifier is about 87%. This is 10% more than logistic regression score. So this is a best fit model when compared.
The model accuracies are 78 percent which means that if we provide a new instance to the model it classifies e-permit or further review accurately 78 percent of the time.
