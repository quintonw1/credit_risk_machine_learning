# Challenge 17 - Supervised Machine Learning for Credit Risk 
Machine learning was implemented to build a mathematical model to predict whether or not someone is a good or bad credit risk given various user traits and loan history.

The analysis was separated into two sections, the first consisting of an undersampling with cluster centroid algorithmn, oversampling with the random oversampler and SMOTE algorithmn, and a combination of the two using the SMOTEENN algorithmn. The second consisting of the balanced random forest classifier, and easy esemble classifier algorithmns. Each algorithmn within each section was then compared to determine which algorithmn best fitted and predicted the data. Additionally, it was noticed that there seemed to be redundant information within the dataset and the impact that removing this data had on the final results was also compared. 

Section 1: 

The following results were obtained for the fitting of the datasets using the section 1 algorithmns listed above. 

Unfiltered:

Oversampling with Random Oversampler: 
Accuracy Score: 0.7237
Low_Risk Precision Score: 1.00
Low_Risk Recall Score: 0.72
High_Risk Precision Score: 0.02 
High_Risk Recall Score: 0.72

Oversampling with SMOTE: 
Accuracy Score: 0.7253
Low_Risk Precision Score: 1.00
Low_Risk Recall Score: 0.73
High_Risk Precision Score: 0.02 
High_Risk Recall Score: 0.72

Undersampling with Cluster Centroid Algorithmn: 
Accuracy Score: 0.7016
Low_Risk Precision Score: 1.00
Low_Risk Recall Score: 0.66
High_Risk Precision Score: 0.01 
High_Risk Recall Score: 0.74

Over/Undersampling with SMOTEENN: 
Accuracy Score: 0.7391
Low_Risk Precision Score: 1.00
Low_Risk Recall Score: 0.73
High_Risk Precision Score: 0.02 
High_Risk Recall Score: 0.75

Filtered:

Oversampling with Random Oversampler: 
Accuracy Score: 0.7233
Low_Risk Precision Score: 1.00
Low_Risk Recall Score: 0.72
High_Risk Precision Score: 0.02 
High_Risk Recall Score: 0.72

Oversampling with SMOTE: 
Accuracy Score: 0.7307
Low_Risk Precision Score: 1.00
Low_Risk Recall Score: 0.73
High_Risk Precision Score: 0.02 
High_Risk Recall Score: 0.73

Undersampling with Cluster Centroid Algorithmn: 
Accuracy Score: 0.7024
Low_Risk Precision Score: 1.00
Low_Risk Recall Score: 0.66
High_Risk Precision Score: 0.01 
High_Risk Recall Score: 0.74

Over/Undersampling with SMOTEENN: 
Accuracy Score: 0.7395
Low_Risk Precision Score: 1.00
Low_Risk Recall Score: 0.73
High_Risk Precision Score: 0.02 
High_Risk Recall Score: 0.75

As shown above, the filtered results performed better than the unfiltered results implying that the algorithmns of question may not be taking into account the redundancies within the data and as a result it is having a negative impact on the accuracy of the models. For a credit risk algorithmn, one would ideally want to be able to have the highest precision and recall numbers, but this isn't realistic. Instead, in order to operate the company in a low risk manner the 
Section 2: 

Unfiltered: 

Balanced Random Forest Classifier: 
Accuracy Score: 0.7334
Low_Risk Precision Score: 1.00
Low_Risk Recall Score: 0.84
High_Risk Precision Score: 0.02 
High_Risk Recall Score: 0.62

Easy Ensemble AdaBoost Classifier: 
Accuracy Score: 0.9335
Low_Risk Precision Score: 1.00
Low_Risk Recall Score: 0.95
High_Risk Precision Score: 0.09 
High_Risk Recall Score: 0.92

Filtered: 

Balanced Random Forest Classifier: 
Accuracy Score: 0.7619
Low_Risk Precision Score: 1.00
Low_Risk Recall Score: 0.86
High_Risk Precision Score: 0.03 
High_Risk Recall Score: 0.66

Easy Ensemble AdaBoost Classifier: 
Accuracy Score: 0.9335
Low_Risk Precision Score: 1.00
Low_Risk Recall Score: 0.95
High_Risk Precision Score: 0.09 
High_Risk Recall Score: 0.92

