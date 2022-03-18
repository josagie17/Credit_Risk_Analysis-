Overview of the analysis:

Credit risk classification is fundamentally uneven, since good loans far outweigh dangerous loans. As a result, additional strategies will be needed to train and assess models with imbalanced classes. Jill requested that I develop and analyse models utilising resampling using the imbalanced-learn and scikit-learn libraries.

I'll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids method, utilising the credit card credit dataset from LendingClub, a peer-to-peer lending services firm. Then, using the SMOTEENN method, I'll utilise a combinatorial strategy of over- and undersampling. Then, to forecast credit risk, I'll evaluate two new machine learning models that eliminate bias, BalancedRandomForestClassifier and EasyEnsembleClassifier. When I'm through, I'll assess the models' performance and offer a written recommendation on whether or not they should be utilised to predict credit risk.
Results:

Accuracy Score:

    Score for Nave Random Oversampling Accuracy: 0.6405 = 64%

    Oversampling Accuracy Score for SMOTE: 0.6585 = 66%

    Score for Undersampling Accuracy: 0.6585 = 66%

    Sampling Accuracy Score for Combination (Over and Under): 0.5442 = 54%

    Accuracy of the Balanced Random Forest Classifier: 0.7959 = 80%

    Accuracy of the Easy Ensemble AdaBoost Classifier: 0.9197 = 91 percent

Score of precision:

    Precision Score of Nave Random Oversampling: 99 percent

    Oversampling Precision Score for SMOTE: 99 percent

    Preciseness of undersampling: 99 percent

    Sampling Precision Score for Combination (Over and Under): 99 percent

    Precision Score of Balanced Random Forest Classifier: 99 percent

    Precision Score of Easy Ensemble AdaBoost Classifier: 99 percent

Score for Recall (Sensitivity):

    Sensitivity of Nave Random Oversampling: 0.56 = 56 percent

    SMOTE Sensitivity Score for Oversampling: 0.69 = 69 percent

    Sensitivity Score for Undersampling: 0.40 = 40%

    Sensitivity Score for Combination (Over and Under) Sampling: 0.57 = 57 percent

    Sensitivity Score of the Balanced Random Forest Classifier: 0.91 = 91 percent

    Sensitivity Score of the Easy Ensemble AdaBoost Classifier: 0.94 = 94 percent

F1 Score:

    F1 Score of Nave Random Oversampling: 0.71 = 71 percent

    SMOTE Oversampling F1 Score: 0.81 = 81 percent -SMOTE Oversampling F2 Score: 0.81 = 81 percent -SMOTE Overs

    F1 Score: 0.56 = 56 percent undersampling

    F1 Score: 0.72= 72 percent -Combination (Over and Under) Sampling

    F1 Score of the Balanced Random Forest Classifier: 0.95 = 95%

    F1 Score of the Easy Ensemble AdaBoost Classifier: 0.97 = 97 percent

Summary:

Based on the accuracy ratings above, we can see that the AdaBoost Classifier machine learning model had the highest rate of accuracy, predicting the correct values 91% of the time. Individually, the resampling models had equal accuracy values of 64 to 66 percent, with the Smote oversampling and undersampling strategies obtaining the same accuracy score.

The precision ratings for all six machine learning models came out to be the same: 99 percent. This indicates that machine learning models can almost always anticipate a positive categorization. However, the accuracy score by itself can only tell us so much, thus it must be combined with the sensitivity score. The sensitivity scores basically tell us how accurate our tests are in predicting the condition, or how fine-tuned the likelihood of a positive test is when the disease is actually present.

Each model's F1 score basically tells us whether there is a significant imbalance between sensitivity and accuracy; a significant imbalance will result in a low F1 score. We can see that resampling methods fall short when compared to Ensemble Classifier machine learning models, with undersampling having the lowest F1 score of 0.56 and the Easy Ensemble AdaBoost Classifier having the highest F1 score of 0.97, demonstrating the least disparity between sensitivity and precision.

It is my proposal that the Easy Ensemble AdaBoost Classifier machine learning model be used to forecast credit risk based on the results and additional data analysis. It constantly received the greatest ratings, especially in terms of accuracy, precision, and sensitivity, and hence successfully predicted the outcomes when compared to the other models.
