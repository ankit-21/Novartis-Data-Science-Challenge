# Novartis-Data-Science-Challenge
## Predict if the Server will be Hacked
This problem represented a very famous type of Machine Learning problems. The imbalanced class problem creates a new kind of problem in machine learning techniques as the conventional models score the model on the basis misclassification of classes and do not take into account the class imbalance. The better metric to measure accuracy of the model in these cases is ROC. Precision and Recall give us a better sense of misclassification of different classes. In this project I tried various methods to deal with imbalance class problems.
## XGBoost
This tree based ensemble algorithm has a parameter 'scale_pos_weight' that penalizes the misclassification of the minority class more than the majority class and makes the model more sensitive towards class imbalance.
## SVM
Similar to XGBoost, this ML technique also has a parameter 'class_weight' that penalizes the misclassification of the minority class more than the majority class.

## imblearn Library
## Random Over-Sampling
This method selects the minority class of the target feature and balances it with the number of samples in the majority class by picking samples at random with replacement from the minority class.
## SMOTE (Synthetic Minority Oversampling Technique)
This method synthesizes elements for the minority class, based on those that already exist. It works by randomly picking a point from the minority class and computing the K-Nearest Neighbors for this point. The synthetic points are added between the chosen point and its neighbors.
## Tomek Links (Under-Sampling the Majority Class)
Tomek links are pairs of very close instances, but of opposite classes. Removing the instances of the majority class of each pair increases the space between the two classes, facilitating the classification process.
## SMOTETomek
This method does a combination of over-sampling and under-sampling, using the SMOTE and Tomek links technique.
