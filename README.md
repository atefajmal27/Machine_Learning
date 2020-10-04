# Machine Learning- Risk Analysis
![](https://user-images.githubusercontent.com/62320593/95018376-525c2e80-062d-11eb-9de6-c5bbf0b1f436.jpg)

## Background 
Auto loans, mortgages, student loans, debt consolidation ... these are just a few examples of credit and loans that people are seeking online. Peer-to-peer lending services such as LendingClub or Prosper allow investors to loan other people money without the use of a bank. However, investors always want to mitigate risk, so you have been asked by a client to help them use machine learning techniques to predict credit risk.

## My Solution 
To solve this issue, I built and evaluated several machine-learning models to predict credit risk using free data from LendingClub. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so I needed to employ different techniques for training and evaluating models with imbalanced classes. I have used the imbalanced-learn and Scikit-learn libraries to build and evaluate models using the two following techniques:

1. Resampling: I used the imbalanced learn library to resample the LendingClub data and build and evaluate logistic regression classifiers using the resampled data.

Steps:

  1. Load the Lending Club data, split the data into training and testing sets, and scale the features data.
  2. Oversample the data using the Naive Random Oversampler and SMOTE algorithms.
  3. Undersample the data using the Cluster Centroids algorithm.
  4. Over- and under-sample using a combination SMOTEENN algorithm.
 
For each of the above, I:

  1. Trained a logistic regression classifier from sklearn.linear_model using the resampled data.
  2. Calculated the balanced accuracy score from sklearn.metrics.
  3. Calculated the confusion matrix from sklearn.metrics.
  4. Printed the imbalanced classification report from imblearn.metrics.


2. Ensemble Learning: For this part, I trained and compared two different ensemble classifiers to predict loan risk and evaluate each model. I used the Balanced Random Forest Classifier and the Easy Ensemble Classifier.

For each model, I:

  1. Loaded the Lending Club data, split the data into training and testing sets, and scaled the features data.
  2. Trained the modeled using the quarterly data from LendingClub.
  3. Calculated the balanced accuracy score from sklearn.metrics.
  4. Printed the confusion matrix from sklearn.metrics.
  5. Generated a classification report using the imbalanced_classification_report from imbalanced learn.
  6. Printed the feature importance sorted in descending order along with the feature score.
