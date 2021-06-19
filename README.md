# Credit-Risk-Resampling - Machine Learning Homework

Background
Auto loans, mortgages, student loans, debt consolidation are just a few examples of credit and loans that people are seeking online. Peer-to-peer lending services such as LendingClub or Prosper allow investors to loan other people money without the use of a bank. However, investors always want to mitigate risk, so you have been asked by a client to help them use machine learning techniques to predict credit risk.

In this assignment, you will build and evaluate several machine-learning models to predict credit risk using free data from LendingClub. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so you will need to employ different techniques for training and evaluating models with imbalanced classes. You will use the imbalanced-learn and Scikit-learn libraries to build and evaluate models using the two following techniques:

Resampling
Ensemble Learning
Files
Resampling Starter Notebook

Ensemble Starter Notebook

Lending Club Loans Data

Instructions
Resampling
You will use the imbalanced learn library to resample the LendingClub data and build and evaluate logistic regression classifiers using the resampled data.

You will:

Oversample the data using the Naive Random Oversampler and SMOTE algorithms.
Undersample the data using the Cluster Centroids algorithm.
Over- and under-sample using a combination SMOTEENN algorithm.
For each of the above, you will need to:

Train a logistic regression classifier from sklearn.linear_model using the resampled data.
Calculate the balanced accuracy score from sklearn.metrics.
Calculate the confusion matrix from sklearn.metrics.
Print the imbalanced classification report from imblearn.metrics.
Use the above to answer the following:

Which model had the best balanced accuracy score?

Which model had the best recall score?

Which model had the best geometric mean score?

Ensemble Learning
In this section, you will train and compare two different ensemble classifiers to predict loan risk and evaluate each model. You will use the balanced random forest classifier and the easy ensemble AdaBoost classifier.

Be sure to complete the following steps for each model:

Train the model using the quarterly data from LendingClub provided in the Resource folder.
Calculate the balanced accuracy score from sklearn.metrics.
Print the confusion matrix from sklearn.metrics.
Generate a classification report using the imbalanced_classification_report from imbalanced learn.
For the balanced random forest classifier only, print the feature importance sorted in descending order (most important feature to least important) along with the feature score.
Use the above to answer the following:

Which model had the best balanced accuracy score?

Which model had the best recall score?

Which model had the best geometric mean score?

What are the top three features?

Hints and Considerations
Use the quarterly data from the LendingClub data that is provided in the Resources folder. Keep the file in the zipped format and use the starter code to read the file.

Refer to the imbalanced-learn and scikit-learn official documentation for help with training the models. Remember that these models all use the model->fit->predict API.

For the ensemble learners, use 100 estimators for both models.

Submission
Create Jupyter notebooks for the homework and host the notebooks on GitHub.
Include a markdown that summarizes your homework and include this report in your GitHub repository.

Findings: Of the three aproaches, the oversampling models had the highest balanced accuracy scores, with naive oversampling the highest at 0.63.
In terms of recall, again, oversampling had the highest scores - this time SMOTE the highest with 0.67.
Oversampling was also highest for geometric mean, with naive oversampling the highest with a score of 0.63.
Credit Risk Ensemble
For the ensemble models, I was sure to scale my data before to achieve better results.

Of the two models, the Easy Ensemble AdaBoost Classifier had the higher balanced accuracy score of 0.945.
The Easy Ensemble Classifier also had the better recall, with a weighed average score of 0.94.
Geometric mean was not reported in the classification report, but the Easy Ensemble Classifier had the higher F1 score of 0.97 (weighted average).
For the balanced random forest model, the top three features were:
Total Received Principal (0.08)
Last Payment Amount (0.068)
Total Received Interest (0.064)
