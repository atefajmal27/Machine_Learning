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




2. Ensemble Learning
