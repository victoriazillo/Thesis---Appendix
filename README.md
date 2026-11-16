# Thesis---Appendix
This is the Appendix of the thesis "Local shrinkage of uncertain predictions based on effective sample size"
## Purpose of this repository
This repository contains the code files used to perform the analyses presented in this thesis.

## How to run the scripts
I suggest to run the Rcode in the order the files are presented below. The local shrinkage algorithm steps are commented in detail in the file 'Model 1- Cross Validation.Rmd' and in the file 'Model 1- Predictions.Rmd'. 
## R code files 

1. The file 'neff exploration linear models.Rmd' contains the code used to explore the effective sample size distributions across different linear model specifications. 

2. The fold 'Cross Validation and Predictions' contains one fold 'Model 1' with two R Markdown files:

- Model 1 - Cross Validation.Rmd: contains the implementation of the local shrinkage algorithm, adapted to perform cross-validation for Model 1.

- Model 1 - Predictions.Rmd: contains the code used to calculate the predictions for Model 1 using OLS , ridge regression and local shrinkage methods.

It also contais the fold 'Model 2, Model 3 and Model 4'  which contains the rmd files where CV and predictions are computed for the three models (2,3 and 4).


3. The file 'Binary predictor shrinkage.Rmd' explores the shrinkage of asymmetric binary predictors using the local shrinkage algorithm.

4. The fold 'Simulation study - model 1' contains the comparison of predictions between methods (local shrinkage - ridge regression - OLS) for model 1 in a simulated setting (Rmd file) and the CSV file where simulated predictions for the local shrinkage algorithm were saved.
5. The fold 'Simulation study - model 4' contains the simulation study (Rmd and CSV file) for model 4
## Which R packages are required.

    library(caret)
    library(Hmisc)
    library(ggplot2)
    library(MASS)
    library(dplyr)
    library(glmnet)



