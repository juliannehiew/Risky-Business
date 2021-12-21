# Risky-Business


Overview of the Analysis:

In this analysis, several machine learning models are built based on the data provided to help predicting whether a customer is at low or high credit risk. Libraries including imbalanced-learn and Scikit-learn are built, along with evaluation models and these techniques, namely Reampling and Ensemble Learning, are applied. In the first couple of models I oversampled the data using randomoversampler and smote algorithms and undersample the data with the clustercentroid algorithm. In the remaining models I used a combination approach to over and undersample the data using smoteenn. Finally, I compared two machine learning models that minimize bias, balancedrandomforestclassifier and easyensembleclassifier.  

## Results:

Naive Random Oversampling results: Balanced accuracy score is 99%, the precision for the high_risk has a very high positivity at 85% and the recall is 100%


## ![Naïve Random Oversampling](https://github.com/juliannehiew/Risky-Business/blob/main/Images/Naive%20Random%20Oversampling.JPG)



SMOTE oversampling results: the accuracy score is 99.4%, the precision for the high_risk loans has a high positvity again at 86% and recall is 99% overall


## ![SMOTE oversampling](https://github.com/juliannehiew/Risky-Business/blob/main/Images/SMOTE%20Oversampling.JPG)



Undersampling results: balanced accuracy score is 98.2% overall, the precision is at 99% and the recall is 99%


## ![Undersampling](https://github.com/juliannehiew/Risky-Business/blob/main/Images/Undersampling.JPG)




Combination(over and undersampling) results: balanced accuracy score is 99.4% the precision is 100% and the recall is 99% overall

## ![Combination](https://github.com/juliannehiew/Risky-Business/blob/main/Images/Combination.JPG)




Balanced Random Forest Classifier results: the accuracy score is 78.9% the precision is 99% and the recall is 89%


## ![Combination](https://github.com/juliannehiew/Risky-Business/blob/main/Images/Balanced%20Random%20Forest.JPG)




Easy Ensemble Classifier results: the accuracy score is 91.7% the precision is 99% and the recall is 89%


## ![Easy Ensemble](https://github.com/juliannehiew/Risky-Business/blob/main/Images/Easy%20Ensemble%20Classifier.JPG)



## Summary:
The first four models demonstrate undersampled, oversampled and a combination of both to determine which model is best at predicting which loans are considered as the highest risk. The latter two models used in resampling the data based on ensemble classifiers aim to predict which loans are at high or low risk.  In essence, it is recommended to achieve a good balance of recall and precision from the first four models. It appears that the Combination had the best balance of all the models due to it's high accuracy score, along with a good balance of precision and recall scores.
