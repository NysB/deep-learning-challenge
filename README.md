# Deep Learning Challenge
This repository contains my homework for Module 21.

The task was to create a model to predict whether an applicant will be succesful if funded by Alphabet Soup. 

## Attachments
In this repository, you will find:
- a file called "Starter_Code.ipynb", with the code written for this assignment;
- a file called "AlphabetSoupCharity_Optimization.h5" with the deep learning model. 

## Result
Furthermore, I have been asked to summarize the outcome in a report. Please see below


### Report: Analysis of Funding Applicant Selection using Deep Learning

#### Overview of the Analysis

The purpose of this analysis is to develop a machine learning module for Alphabet Soup, a nonprofit foundation, to support their selection of funding applicants with the highest probability of success in their ventures. 

#### Result

##### Data Preprocessing

Target Variable: The target variable for the model is the "IS_SUCCESSFUL" column, which indicates whether the funding was used effectively (1) or not (0).

Features: The features for the model include the following columns:
- APPLICATION_TYPE: Alphabet Soup application type;
- AFFILIATION: Affiliated sector of industry;
- CLASSIFICATION: Government organization classification;
- USE_CASE: Use case for funding;
- ORGANIZATION: Organization type;
- INCOME_AMT: Income classification;
- ASK_AMT: Funding amount requested.

Variables to be removed: The "EIN," "NAME", and "SPECIAL_CONSIDERATIONS" headers were removed as they were not directly linked to the probability of success. EIN and NAME are solely used to identify the company, which does not help the performance of the model. In addition, SPECIAL CONSIDERATIONS did not improve the accuracy of the model and therefore was removed from the dataset.  

##### Compiling, Training, and Evaluating the Model

Neurons, Layers, and Activation Functions: The deep neural network model consists of five layers. The architecture is as follows:

- Layer 1: 20 nodes with the ReLU activation function;
- Layer 2: 15 nodes with the ReLU activation function;
- Layer 3: 10 nodes with the tanh activation function;
- Layer 4: 10 nodes with the tanh activation function;
- Output Layer 5: 1 node with the sigmoid activation function.

Target Model Performance: The model achieved a loss of 0.5566 and an accuracy of 0.7312.

##### Steps to Increase Model Performance: Further attempts can be made to enhance the model's performance by:

The model resulted in a loss of 0.5566 and an accuracy of 0.7289. Although the target of 75% accuracy waas not reached, the model achieved a reasonably good performance.

The following steps were taken to improve performance:
- I experimented with the number of nodes and layers;
- I experimented with using different activitation functions;
- Initially I left the "STATUS" and "SPECIAL_CONSIDERATIONS" columns in the data, but that resulted in a lower performance. 

