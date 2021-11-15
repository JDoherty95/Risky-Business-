# Risky-Business-
From the results, all four resampling alogorithms had very low precision rates classifying observations as high credit risk. Each model scored fairly well in identifying above 70% of actual high credit risk observations based on the high risk recall scores, but misclassified low credit risk observations as high credit risk, resulting in a low precision rate for high risk.

On the flip side, precision scores were very high for low risk as the models all performed well in correctly classifying low credit risk out of the total low credit risk the model identified.

The recall scores were all similar, except for Cluster Centroids. Undersampling the data improved the recall score of high risk but offset by a lower recall of low risk.

*In conclusion, all models performed fairly well in correctly classifying high credit risk and low credit risk observations, but all models had high error rates misclassifying low credit risk as high credit risk. SMOTE marginally performed best across all metrics.

Resampling Algorithms	Precision Score / High Risk	Precision Score / Low Risk	Recall / High Risk	Recall / Low Risk
Naive Random	0.01	1.00	0.70	0.69
SMOTE	0.02	1.00	0.71	0.73
Cluster Centroids	0.01	1.00	0.82	0.47
SMOTEENN	0.01	1.00	0.74	0.65
Total Score Summary

Resampling Algorithms	Balanced Accuracy	Recall Score	F1 Score	Geometric Mean Score
Naive Random	70.0%	0.69	0.81	0.70
SMOTE	72.0%	0.73	0.84	0.72
Cluster Centroids	65.0%	0.48	0.64	0.62
SMOTEENN	69.0%	0.65	0.78	0.69

Ensemble Classifiers	Precision Score / High Risk	Precision Score / Low Risk	Recall / High Risk	Recall / Low Risk
Balanced Random Forest	0.09	1.00	0.66	0.89
Easy Ensemble	0.09	1.00	0.92	0.94
Total Score Summary

Resampling Algorithms	Balanced Accuracy	Recall Score	F1 Score	Geometric Mean Score
Balanced Random Forest	78.0%	0.89	0.93	0.77
Easy Ensemble	93.0%	0.94	0.97	0.93
The top three features from the Balanced Random Forest:

