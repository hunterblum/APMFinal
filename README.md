# Afraid of Needles? Machine Learning Might Help to Determine Your LDL Levels
## This project is a part of the ADS-503 course in the Applied Data Science Program at the University of San Diego. 
## Final Project for ADS 503 Team 1 (Summer 2022)
## Partner(s)/Contributor(s)  
•	Brianne Bell, Eva Chow, Hunter Blum

-- Project Status: [Completed]

# Installation
Code files can be run in R Studio. There is a Java or R or Windows conflict with RWeka library which makes RWeka code not runnable in all instances, check to see if it runs (if it will not, it restarts R). The models developed are not currently recommended for use outside of classroom modeling practice/understanding.

# Project Intro/Objective
The main purpose of this project is to explore different modeling methods to develop the best model for predicting LDL levels from demographic and biological measures. By developing this model, patients could avoid being unnecessarily poked to have their blood drawn to check LDL cholesterol levels. This would alleviate costs to the clinic, laboratory, insurance, and patient. This would also alleviate patient nerves by reducing time around needles to only when necessary (i.e. a high or concerning LDL level is predicted). 

# Methods Used
•	Exploratory Data Analysis (EDA)
•	Linear Regression Models
•	Non-Linear Regression Models
•	Regression Tree Models
•	Data Imputation
•	RMSE score comparisons
•	Data Visualization

# Technologies
•	R

# Project Description
The ultimate goal is to isolate a model capable of predicting LDL levels with reasonable reliability, based on RMSE value. The data was sourced from the National Health and Nutrition Examination Survey (NHANES) pre-pandemic data set, which included observations from 2017 to March of 2020. The datasets used were the demographic, body measurements, and LDL (low-density lipoproteins aka bad cholesterol) datasets. The demographic and body measurements datasets were left joined to the LDL observations. Variables relating to physician comments or with high (>1000) missing values were removed. Additionally, variables with near zero variation were removed as well as those with high correlations. The categorical features were replaced with dummy columns for modeling purposes. 

The data was split so that 80% went to training models while 20% were held in reserve for testing the models. Several models were explored from the linear regression, non-linear regression, and regression tree model families. These were optimized during training to select the parameters with the lowest RMSE value. The best models of each family of regression model type and the best overall model was also determined. These final determinations were based on the RMSE of the test data being processed through the tuned models. 

# License
Data is open source and came from the National Health and Nutrition Examination Survey (NHANES) pre-pandemic data set, which included observations from 2017 to March of 2020.

# Acknowledgments
