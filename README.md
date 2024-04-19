# SC1015 Mini Project

This repository contains the Jupyter Notebook files and the data set for the Mini Project for NTU's SC1015 module.

The *data* folder contains the original data set, and the pickle files for the used to transfer DataFrames resulting from the data preparation and data exploration.

The external libraries used are indicated in the requirements.txt file. To install the required libraries, run the following command:

> pip install -r requirements.txt

---

**Table of Contents:**

1. [Group Info](#group-info)
2. [Problem Statement](#problem-statement)
3. [Data Preparation](#data-preparation)
4. [Exploratory Analysis](#exploratory-analysis)
5. [Modelling](#modelling)
6. [Conclusions](#conclusions)
7. [What we learned](#what-we-learned)
8. [References](#references)

## About our Project

Predicting the potential of contracting cardiovascular disease using the following dataset obtained from kaggle:
https://www.kaggle.com/datasets/jocelyndumlao/cardiovascular-disease-dataset

### Group Info
<u>Lab Group:</u> FCEA

Team 9:
- Ariel Kwok Dai Hui
- Liong XunQi
- Le Nguyen Bao Huy

### Problem Statement

Using the data set, we aim to answer the following questions:
- Which factors are indicators of cardiovascular diseases
- Are the elderly more likely to get cardiovascular diseases

### Data Preparation

The data set has 1000 rows and 14 features. Using patient IDs, we concluded there were no duplicate data in the data set. We also found that there were no missing values in the data set. 

The *patientid* feature was dropped from the data set because it was irrelevant to the analysis. Categorical variables like *slope* or *chestpain* were split using one hot encoding.

Other changes to the data set include changing column data types to boolean for compactness and clarity, as some name changes to make certain information more clear.

### Exploratory Analysis



### Modelling

From the dataframe obtained after the data exploration process, we can build several models for predicting the presence of cardiovascular diseases.

Before that, to ensure to able to recreate the models, we initially randomly selected a seed value, and then passing to the *random_state* parameter for any models which accepted it.

We fit the data into the a Logistic Regression model, a Decision Tree Classifier model and a Random Forest Classifier model. In particular, we hypertuned the parameters of the Random Forest model using grid search and cross validation techniques.

We found that the Random Forest Classifier model had the highest accuracy out of all of them, but also took the longest to execute the underlying code.

### Conclusions

### What we learned

Through this project we learned how to collaborate with each other effectively for a coding project and other techniques for conducting data analysis:
- Saving dataframe to pass to other members for next steps of data analysis through .pkl files
- Using GitHub to collaborate with each other effectively.
- Using Logistic Regression to predict whether subject has cardiovascular disease or not.
- Using RandomForest and hypertuning parameters to find the best model for predicting.

### References

https://www.kaggle.com/datasets/jocelyndumlao/cardiovascular-disease-dataset