Steps performed in Model Evaluation

* Inspecting the data and splitting the data into training amnd test sets.
* Creating a pipeline to perform feature processing
* Creating a logistic regression model pipeline that uses the above pipeline
* Picking up a matric for selecting the model
* With the combined pipeline running a Logistic Regression model with grid search cross-validation
* Concluding which is the best model and performance on the test set¶

After checking if there are anyb missing values, it ois found that there are nio missing values inm the dataset. So we need not to perform any inmpute functiuon.
We divided the data into training and test using train_test_split from sklearn.model_selection.
As we have only numerical values in the dataset, we use StandardScaler()
We attain the modeling pipeline with logistin regresion and penalty as none.
We get the model pipeline with metrics precision, recall, f1 score and accuracy.
We implement roc curve and estimate the performance.

Here we use the recall metric.This quantifies the number of correct positive predictions made out of all positive predictions that could have been made. Unlike precision that only comments on the correct positive predictions out of all positive predictions, recall provides an indication of missed positive predictions.¶

using the solver 'liblinear' with l2 penalty with 5 different regulization strenghths, we perform Grid search
We use the solvers 'saga' and 'liblinear' and estimate performance of each model.

In the result, we find that after using both the solvers on test set, we observe that the values of all the metrics remain same. So both the models are best fit for the Evaluation.
