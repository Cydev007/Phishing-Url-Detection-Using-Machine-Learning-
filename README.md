# Phising-Url-Detection-Using-Machine-Learning-

Phishing is one of the internet security problems that target the human vulnerabilities rather than software vulnerabilities.

## Introduction
Phising attack can be described as the process of attracting online users to obtain their sensitive information such as usernames and passwords. Phishers try to deceive their victims by social engineering or creating mockup websites to steal information such as account ID, username, password from individuals and organizations. 

## Objective
The objective of this project is to train machine learning models and deep neural network on the dataset created to predict phishing websites. Both phishing and legitimate URLs of websites are gathered to form a dataset and from them required URL and basic features are extracted. 

## Data Collection
**URL Dataset**
The set of phishing and Legitimate URLs are collected from opensource service called **Kaggle** , **Phistank** , **Phistrom**. These service provide a set of phishing  and legitimate URLs in multiple formats like csv, json etc. I combined the data from these services. From this dataset, 549347 random phishing and legitimates URLs are collected to train the ML models and they are labeled as Good and Bad.

The above mentioned datasets are uploaded to (dataset url) folder of this repository.

## Preprocessing
Data preprocessing can refer to manipulation or dropping of data before it is used in order to ensure or enhance performance, and is an important step in the data mining process. I use RegexpTokenizer  to tokenized words. And use CountVectorizer  to transform a corpora of text to a vector of term / token counts.

## Models & Training

Before stating the ML model training, the data is split into train and test dataset. From the dataset, it is clear that this is a supervised machine learning task. There are two major types of supervised machine learning problems, called classification and regression. 

This data set comes under regression problem, as the input URL is classified as good or bad. The supervised machine learning models (regression) considered to train the dataset in this project are:

* Logistic Regression

All these models are trained on the dataset and evaluation of the model is done with the test dataset. 

## Prediction

I store the trained data in .pkl file and use it for predict urls are legitimate or phishing.


## **Tools Used**
->Jupyter notebook 
->Pycharm 
->Brave Browser 


->>> Documentation
The Write-up Documentation for this project is named "DETECTING PHISHING URLs USING MACHINE LEARNING.pdf"


-> ML work 
The ML work folder consist of "Dataset" and "Jupyter notebook of the project" as stated above 
** Phishing Website Detection Training & Testing Models on Datasets.ipynb **
** URL_Feature_Extraction_from_Datasets.ipynb **

-> Extend This Project
I will use nural network and deep learing techniques to predict urls more accurately. Project can be further extended to creation of browser extention (for chrome, brave, Firefox etc) to help Users by adding it to browser extension to detect Phishing URLs .