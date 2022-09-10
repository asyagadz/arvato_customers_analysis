# Arvato Customer analysis
This project is the Capstone project under the Udacity Data Science Nanodegree program.

## Installations
cycler==0.10.0
matplotlib==3.5.2
numpy==1.23.1
pandas==1.4.3
scikit_learn==1.1.1
seaborn==0.11.2
xgboost=1.6.2

There is a requirements.txt file in the main project.


## Project Motivation
This is the final project to complete the Udacity Data Science Nanodegree program.
The scope of the project is divided into 2 parts:
1. Customer segmentation analysis: we are using 2 datasets - demographics data of the general population in Germany, and demographics data of Arvato's customers, to segment the population into clusters, and provide insights to which segments the customers of the company belong to, along with the demographic features that define those segments. 
2. Classification analysis, whose purpose is to build a model to predict which individuals are most likely to become customers of the company. For this puprose, a training dataset with demographics information for targets of the marketing campaign for the company was provided, along with a test dataset for which we predict the probability of becoming a customers.
 The final output of this part of the analysis is a csv file with probabilities how likely for each individual from the test dataset is to become a customer to the company.


## File Descriptions
The project contains:
- A Readme.md file
- Notebooks folder
  - 01.01.-ag-cluster-classification.ipynb - all code and work is done within this notebook
- src folder:
  - data:
    - raw data - the raw files as downloaded from Udacity, but are not presented in the current repository, because they are too big:

  --- Udacity_AZDIAS_052018.csv: Demographics data for the general population of Germany; 891 211 persons (rows) x 366 features (columns).<br>
  --- Udacity_CUSTOMERS_052018.csv: Demographics data for customers of a mail-order company; 191 652 persons (rows) x 369 features (columns).<br>
  --- Udacity_MAILOUT_052018_TRAIN.csv: Demographics data for individuals who were targets of a marketing campaign; 42 982 persons (rows) x 367 (columns).<br>
  --- Udacity_MAILOUT_052018_TEST.csv: Demographics data for individuals who were targets of a marketing campaign; 42 833 persons (rows) x 366 (columns).<br>
  --- DIAS Attributes - Values 2017.xlsx - information about the attributes/features
  --- DIAS Information Levels - Attributes 2017 - detailed information about the features

    - processed data - the files processed throughtout the different steps of the project.

  - models:

  --- gbmclassifier.pkl - the final classification model
  --- gbc_pred.csv - output of the classification task - the probabilities of becoming a client for each individual from the test set.

## How to Interact with your project/Results
The output of the Clustering part of the analysis are the clusters the general population is divided into based on its demographic characteristics, as well as information to which clusters the customers of the company belong to.

The final output of Classification part of the analysis is a csv file with probabilities how likely for each individual from the test dataset is to become a customer to the company. 


The blog post for the analysis can be found here: https://medium.com/@asya.gadz/a-study-on-airbnb-boston-data-410940343dd8

## Licensing, Authors, Acknowledgements, etc.
I have used some functions or code that is from Feature Engineering course & Feature Selection course from Udemy, lead by Soledad Galli.
