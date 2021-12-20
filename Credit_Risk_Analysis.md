Credit_Risk_Analysis

Overview of the analysis:

Credit risk is very tough to predict. In this project, all factors is taken into considerations in the loan_stats csv help predict whether someone is low or high risk status. One method that data scientists use for this type of issue is creating a model and then evaluate and train the models that they create. In this specific project we are using imbalanced-learn and scikit-learn libraries to build models and evalute them using a resampling method. In the first couple of models I oversampled the data using randomoversampler and smote algorithms and undersample the data with the clustercentroid algorithm. In the remaining models I used a combination approach to over and undersample the data using smoteenn. Finally, I compared two machine learning models that minimize bias, balancedrandomforestclassifier and easyensembleclassifier.

Results:
Naive Random Oversampling results: Balanced accuracy score is 99%, the precision for the high_risk has a very high positivity at 85% and the recall is 100%





SMOTE oversampling results: the accuracy score is 99.4%, the precision for the high_risk loans has a high positvity again at 86% and recall is 99% overall






Undersampling results: balanced accuracy score is 98.2% overall, the precision is at 99% and the recall is 99%







Combination(over and undersampling) results: balanced accuracy score is 99.4% the precision is 100% and the recall is 99% overall







Balanced Random Forest Classifier results: the accuracy score is 78.9% the precision is 99% and the recall is 89%






Easy Ensemble AdaBoost Classifier results: the accuracy score is 91.7% the precision is 99% and the recall is 89%






Summary:
The first four models demonstrate undersampled, oversampled and a combination of both to determine which model is best at predicting which loans are considered as the highest risk. The latter two models used in resampling the data based on ensemble classifiers aim to predict which loans are at high or low risk.  In essence, it is recommended to achieve a good balance of recall and precision from the first four models. It appears that the Combination had the best balance of all the models due to it's high accuracy score, along with a good balance of precision and recall scores.