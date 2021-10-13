Introduction:
We perform regression to predict the value of an entity based on some of the mentioned or definitied values. In the dataset I have taken, it mainly focus on the life expectancy. So here a regression model is created to predict the value of life expectancy. We are going to use OLS regression model and Ridge Model and also compare the coefficients

Operations Performed:

Importing all the required packages Pandas, Numpy, CSV, matplotlib, seaborn

Defining the dataset of Life Expectancy Data of different countries over the years

Droping unnecessary columns in the dataset

Displaying the datatype of all the columns present

Changing the datatype as required for performing Regression Model

Finding the missing values in the dataset

Filling the missing values with the median value

Dispalying the new cleaned dataset

Creating a OLS regression model using Statmodels

Predicting the Life Expectancy value based on the actual value in the dataset

Making it scatter and introducing alpha

Histogram showing distribution of actual and predicted values of Life Expectancy

Splitting the Dataset to Training and Test data

Creating a Pipeline to preprocess the data

Evaluating the model on the test data

Creating a Ridge model

Conclusion:

As there is a drop in the value with increase of alpha, the life nexpectancy may be significantly decreasing and we can expliain the variance totally.
So along the years the life expectancy is being reduced.
