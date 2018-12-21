# Classifier_Python
Simple classification problem: classify type of cancer(benign-malignant) based on 9 attributes.
The dataset information can be found here: https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.names.
The dataset can be found here: https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29.

The accuracy of two different approaches was evaluated.

## Mean_mean_method

The first method reached an accuracy of 0.94. Of 345 total number of cases in the test set there were 20 inaccuracies.

## Logistic regression
The logistic regression method reached the 0.98 accuracy on test dataset.

Report of Logisic Regression method on our dataset:

Confusion Matrix

               [[110   3 ]
                [ 2   107]]
                   
We have 110+107 correct predictions and 2+3 incorrect predictions.
 
Accuracy of logistic regression classifier on test set: 0.98

                  precision    recall  f1-score   support

               b       0.98      0.97      0.98       113
               m       0.97      0.98      0.98       109 
           
       micro avg       0.98      0.98      0.98       222
       macro avg       0.98      0.98      0.98       222
    weighted avg       0.98      0.98      0.98       222

Report legenda from Sklearn:
- The precision is the ratio tp / (tp + fp) where tp is the number of true positives and fp the number of false positives. The precision is intuitively the ability of the classifier to not label a sample as positive if it is negative.
- The recall is the ratio tp / (tp + fn) where tp is the number of true positives and fn the number of false negatives. The recall is intuitively the ability of the classifier to find all the positive samples.
- The F-beta score can be interpreted as a weighted harmonic mean of the precision and recall, where an F-beta score reaches its best value at 1 and worst score at 0.
- The F-beta score weights the recall more than the precision by a factor of beta. beta = 1.0 means recall and precision are equally important.
- The support is the number of occurrences of each class in y_test.


References for the code and the methods:
1. "The practice of computing using Python", 2nd Edition, by William F. Punch (Author), Richard Enbody (Author). ISBN-13: 978-0134380315.
2. "Building A Logistic Regression in Python, Step by Step" by Susan Li https://towardsdatascience.com/building-a-logistic-regression-in-python-step-by-step-becd4d56c9c8. https://datascienceplus.com/building-a-logistic-regression-in-python-step-by-step/. Github: https://github.com/susanli2016/Machine-Learning-with-Python/blob/master/Logistic%20Regression%20balanced.ipynb
3. Chawla, Nitesh V., et al. "SMOTE: synthetic minority over-sampling technique." Journal of artificial intelligence research 16 (2002): 321-357.
