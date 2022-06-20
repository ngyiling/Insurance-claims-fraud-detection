# Insurance Claims Fraud Detection
This project is a fraud classification of an “unbalanced” data set of car insurance claims. The insurance-claims.csv dataset consists of more than 10,000 claims, with only 100 fraudulent claims among all the claims. We carried out pre-processing of the dataset followed by 3 types of classifications: SMOTE, Autoencoder, SMOTE with Decision Tree to identify the best classification model. 

<br />

**Technology:** sklearn, seaborn, matplotlib, pandas, numpy, tensorflow, keras, SMOTE, imblearn

<br />

**Results:** 
- Autoencoder model was identified as the best classification model; it performed better than the SMOTE model with an higher accuracy to recognise differences between patterns.
- The SMOTE training data was used to train the decision tree model. However, the generated datapoint from oversampling influenced the classification of the "fraud" class and gave 293 false positives.
- Hence, the SMOTE model performed better than the decision tree model but worse than the autoencoder model as the autoencoder model has a different approach to rebuilding data. Hence its AUC is relatively better compared to other models.

