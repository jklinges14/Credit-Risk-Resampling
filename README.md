# Credit-Risk-Resampling - Machine Learning Homework

Of the three aproaches, the oversampling models had the highest balanced accuracy scores, with naive oversampling the highest at 0.63.
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
