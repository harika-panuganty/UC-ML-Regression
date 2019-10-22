# ML-Regression

This weekly project for my Intermediate Applied Data Analysis class from the MscBMI Program at The University of Chicago tested on Naive Model, GLM Model, Logistic Regression and Ridge Regression in R. The code for this repository elaborates on the specific code used for Naive Model, GLM Model, Logistic Regression and Ridge Regression Models for three Kaggle datasets in R:

1. A large patient readmission dataset https://inclass.kaggle.com/c/predicting-30-day-hospital-readmissions 

a) Naive Model: using R function GLM with five-fold cross validation. AUC and 95% CI was printed to check accuracy of the model.

b) Logistic Regression: using R function GLM with five-fold cross validation. AUC and 95% CI was printed to check accuracy of the model.

2. A medium sized patient laboratory values dataset  https://www.kaggle.com/c/gusto/data 

a) Logistic Regression: First changed outcome variable to categorical and assigned 'levels', then trained using R function GLM with TrainControl being five-fold cross validation. AUC and 95% CI was printed to check accuracy of the model.

b) Ridge Regression: After changing outcome variable to categorical and assigning 'levels', model trained using R function GLM with TrainControl being five-fold cross validation. For ridge regression model specifically, R function glmnet was used andtook into account the outcome variable with pertinent factors, train data, binomial family and alpha as 0. To select a good lambda value, 5 fold cross validation in glmnet was used and then fine-tuned in caret using R function cv.glmnet. Checking for lambda with minimum deviance, lambda with 1se and created a grid for all the lambda values in between. AUC and 95% CI was printed to check accuracy of the model.

3. A primate junction splice sequence dataset  https://inclass.kaggle.com/c/cs529-project1/data (significant challenges due to nucleotide format of data). This dataset included three outcome variables (IE, EI and N) therefore there are models for each variation of a combination of the three variables. 

a) Logistic Regression: After mutating outcome variable (this way the outcome variable would correspond based on specific lettering), outcome variable was then changed into a factor. R function glm was used to train with trainControl being five-fold cross validation and family as binomial. AUC and 95% CI was printed to check accuracy of the model.

b) Ridge Regression: After mutating outcome variable (this way the outcome variable would correspond based on specific lettering), outcome variable was then changed into a factor. R function glm was used to train with trainControl being five-fold cross validation and family as binomial. For ridge regression model specifically, R function glmnet was used andtook into account the outcome variable with pertinent factors, train data, binomial family and alpha as 0. To select a good lambda value, 5 fold cross validation in glmnet was used and then fine-tuned in caret using R function cv.glmnet. Checking for lambda with minimum deviance, lambda with 1se and created a grid for all the lambda values in between.AUC and 95% CI was printed to check accuracy of the model.
