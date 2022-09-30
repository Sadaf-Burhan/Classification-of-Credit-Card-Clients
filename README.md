# Classification-of-Credit-Card-Clients
## Learning Outcomes


* Data exploration and pre-processing

* Develop a pipeline to carry out classification

* Compare different metrics and classifiers

The objective is to predict whether or not a credit card client will default for their payment in the next month. We will be using the better of 2 classifiers namely, Random Forest and KNN Classifier, and determine the best of a given set of hyperparameters by using grid search.


So in this data set we used Random Forest & KNN classification to predict the credit card default in the next month. For this scenario, a high recall and precision both are very important.As both higher false negative rate or false positive rate may result a huge loss to the bank. In case of wrongly predicting a non defaulting customer as a defaulter, bank may end up loosing valuable customers of future and in case of wrongly predicting a defaulter a non defaulter may cause the bank to default it self.

Therefore the best model should be more concerned with correct prediction of minority class i.e. default next month=1.

Since Sensitivity is the proportion of true positives that are correctly identified, so its higher value is definitely better. We can see that since recall is higher for Random forest therefore also resulting in a smaller value of precision in comparison to the precision score of KNN. So even though KNN has a little higher accuracy than Random forest, but the Recall or sensitivity of Random Forest is better than KNN. Generally when the data is unbalanced like this one, the model performance is better judged by F1 score, which is basically a weighted average of Precision and Recall. Therefore, this score takes both false positives and false negatives into account. And so, f1 score of Random Forest is better than KNN.

This is also evident from area under curve (ROC_AUC_SCORE), as random forest has better ROC_AUC. Also cross validation score of KNN is less than Random Forest, so Random Forest performed better.
