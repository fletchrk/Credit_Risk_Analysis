# Credit_Risk_Analysis
## Overview of Project
This project I will be applying machine learning to solve a real-world challenge: credit card risk. The project has me employ different techniques to train and evaluate models with unbalanced classes. I will be using imbalanced learn and scikit learn libraries to build and evaluate models using resampling.
Using the dataset from LendingClub, which is a peer-to-peer lending services company, I will oversample the data using RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. The next step I will be doing is I will use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. For step 3 I will be comparing two new machine learning models that reduces bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Wrapping up the project I will be evaluating the performance of the models and make a written recommendation on whether they should be used to predict credit risk.

## Results

The Naïve Random Oversampling results are:
•	Balanced accuracy test percent is at 62%
•	Precision for high risk has a very low positivity at 1%
•	Recall is 59%

![Naive_Random_Oversampling]( https://github.com/fletchrk/Credit_Risk_Analysis/blob/main/Resources/Naive_Random_Oversampling.png)

SMOTE Oversampling results are: 
•	Balanced accuracy test percent is at 63%
•	Precision for high risk has a very low positivity at 1%
•	Recall is 62%

![SMOTE_Oversampling]( https://github.com/fletchrk/Credit_Risk_Analysis/blob/main/Resources/SMOTE_Oversampling.png)

Undersampling results are: 
•	Balanced accuracy test percent is at 63%
•	Precision for high risk has a very low positivity at 1%
•	Recall is 63%

![Undersampling]( https://github.com/fletchrk/Credit_Risk_Analysis/blob/main/Resources/Undersampling.png)

Combination (over and undersampling) results are: 
•	Balanced accuracy test percent is at 51%
•	Precision for high risk has a very low positivity at 1%
•	Recall is 70%

![Combination_Over_and_Under_Sampling]( https://github.com/fletchrk/Credit_Risk_Analysis/blob/main/Resources/Combination_Over_and_Under_Sampling.png)

Balanced Random Forest Classifier results are: 
•	Balanced accuracy test percent is at 80%
•	Precision for high risk has a very low positivity at 3%
•	Recall is 71%

![ Balanced_Random_Forest_Classifier]( https://github.com/fletchrk/Credit_Risk_Analysis/blob/main/Resources/Balanced_Random_Forest_Classifier.png)

Easy Ensemble AdaBoost Classifier results are: 
•	Balanced accuracy test percent is at 93%
•	Precision for high risk has a very low positivity at 7%
•	Recall is 91%

![Easy_Ensemble_AdaBoost_Classifier]( https://github.com/fletchrk/Credit_Risk_Analysis/blob/main/Resources/Easy_Ensemble_AdaBoost_Classifier.png)

### Summary
I performed four different undersampling, oversampling and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. The next step was to resample the data using ensemble classifiers to try and predict which loans are high or low risk. In the first four models the accuracy scores were not even close to being as high as the ensemble classifiers. In addition, the recall in the oversampling/undersampling/mixed models is low as well. Normally in the models a good balance of recall and precision is what is looked for. I recommend the ensemble classifiers over the undersampling, oversampling, and combination models. The results show that the Easy Ensemble had the best balance of all the models because of the high accuracy score and good balance of precision and recall scores.

