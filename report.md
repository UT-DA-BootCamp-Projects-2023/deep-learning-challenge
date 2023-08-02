# Alphabet Soup Report using Machine learning and Neural Network

## Overview of the Analysis
--
* The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. Objective of this analysis is using machine learning and neural network for the provided dataset , creating a binary classifier that can predict if the applicants will be successful if funded by Alphabet Soup.

## Steps followed to perform the Analysis
--
* Below are the list of activities performed which would showcase the usage of machine learning and nerual network
  * Preprocessing the data using pandas and scikit-learn's StarndardScaler()
  * As next step, compile, train and evaluating the neural network model. 

## Results
--

### --**Data Preprocessing**-- <br>
* Within this dataset are a number of columns that capture metadata about each organization. These columns used as features and target varibales for this analysis. <br>
<br>

* How each of these are used with this analysis are listed below they are used for this analysis are as follows <br>

  * EIN - Identification column --**Removed**--
  * NAME - Identification column --**Initally Removed but later model retained which improved the accuracy**--
  * APPLICATION_TYPE—Alphabet Soup application type --**Feature Variable**--
  * AFFILIATION—Affiliated sector of industry --**Feature Variable**--
  * CLASSIFICATION—Government organization classification --**Feature Variable**--
  * USE_CASE—Use case for funding --**Feature Variable**--
  * ORGANIZATION—Organization type --**Feature Variable**--
  * STATUS—Active status --**Feature Variable**--
  * INCOME_AMT—Income classification --**Feature Variable**--
  * SPECIAL_CONSIDERATIONS—Special considerations for application --**Feature Variable**--
  * ASK_AMT—Funding amount requested --**Feature Variable**--
  * IS_SUCCESSFUL—Was the money used effectively  --**TARGET Variable**--



How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take in your attempts to increase model performance?


## Summary
--<br>
Both models performed good for health loan status prediction as the precision and recall score is at 100%. Hence the performance between models will be compared against High-risk loan status prediction.<br>
<br>
It is important to have high Precision and high recall values as "A high precision score indicates less false positives and high recall score indicates less false negative. Based on this consideration, RandomOverSampler model seems to perform better when compared to the 'train_test_split' model. Even though the percentage of false positive (precision score) score is same in both the models, RandomOverSampler model showcases better recall score and thus reducing false negative score. Still with only 87% precision rate false positive could lead to potential loss of customer. <br>
<br>
Based on the above explanation I would recommend the `RandomOverSampler` model when compared to '`train_test_split` model due to its improved recall accuracy.