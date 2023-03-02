# Credit_Risk_Analysis

Models of credit risk were created using machine learning methodology. These models predicted high or low risk based on multiple variables in a dataset of approximately
69,000 past instances of loans. A discussion of the effectiveness of the models is provided.

##Models of Analyses
The following models were used with results provided below: Naive Random Sampling, SMOTE Oversampling, Undersampling, Combination (Over and Under) Sampling, Balanced 
Random Forest Classifier, and Easy Ensemble AdaBoost Classifier.

1.Naive Random Oversampling

Balanced Accuracy Score
![image](https://user-images.githubusercontent.com/114311015/222308943-c75eb139-d276-4656-9429-09281f83d365.png)

Confusion Matrix
![image](https://user-images.githubusercontent.com/114311015/222308968-d2bcf45f-7492-49ce-9ea8-803710bb10e1.png)

Imbalanced Classification Report
![image](https://user-images.githubusercontent.com/114311015/222308999-22228fbe-e7d3-47d9-b38e-f74f5fcb260a.png)


2.SMOTE Oversampling

Balanced Accuracy Score
![image](https://user-images.githubusercontent.com/114311015/222308658-05fcf587-e389-4f4d-9643-13f9fd4f877d.png)

Confusion Matrix
![image](https://user-images.githubusercontent.com/114311015/222308689-863d5e8a-44a9-4f1f-885b-9f303e44c34c.png)

Imbalanced Classification Report
![image](https://user-images.githubusercontent.com/114311015/222308740-c56fe27a-e023-45ff-b286-a45a78a171c6.png)


3.Undersampling

Balanced Accuracy Score
![image](https://user-images.githubusercontent.com/114311015/222309072-cd2f1587-5e0f-433b-a7cc-c5edd1ef7a2f.png)

Confusion Matrix
![image](https://user-images.githubusercontent.com/114311015/222309094-8031afcf-ba80-46d5-91ae-b375c3558d6d.png)

Imbalanced Classification Report
![image](https://user-images.githubusercontent.com/114311015/222309137-906fca1a-a56a-4264-88cb-35da8c6027f3.png)


4.Combination (Over and Under) Sampling

Balanced Accuracy Score
![image](https://user-images.githubusercontent.com/114311015/222309245-0d630428-b6ee-4f66-9495-2991d3f7719b.png)

Confusion Matrix
![image](https://user-images.githubusercontent.com/114311015/222309282-b8c5ecc0-5b15-410c-bede-5754d08e3e82.png)

Imbalanced Classification Report
![image](https://user-images.githubusercontent.com/114311015/222309304-e03a71e6-f8b8-4fec-ad25-f7fb069fe268.png)


5.Balanced Random Forest Classifier

Balanced Accuracy Score
![image](https://user-images.githubusercontent.com/114311015/222309551-efc29fc1-0a6a-4615-ae38-db32f631ab52.png)

Confusion Matrix
![image](https://user-images.githubusercontent.com/114311015/222309576-2a70f946-6682-4c1a-8b5f-194607f5321f.png)

Imbalanced Classification Report
![image](https://user-images.githubusercontent.com/114311015/222309597-8771de0b-17d5-4470-8fae-6750ab24a5e4.png)


6.Easy Ensemble AdaBoost Classifier

Balanced Accuracy Score
![image](https://user-images.githubusercontent.com/114311015/222309696-dd1420a0-3828-4956-a39f-62fd224dccf9.png)

Confusion Matrix
![image](https://user-images.githubusercontent.com/114311015/222309722-980b7116-7a06-4721-a63c-67f164e6066a.png)

Imbalanced Classification Report
![image](https://user-images.githubusercontent.com/114311015/222309747-cce56fbc-ed99-4a05-926a-5067823dac97.png)

##Summary

The results indicate that the first four methods can be rejected based on accuracy scores. In particular the Combination (Over and Under) Sampling method model is only
slightly more accurate than flipping a coin. While all of the first four analyses created model were precise in indentifying low-risk loans they were extremely in precise
at identifying high risk loans. Thus the recall rates on identifying low-risk loans ranged from .60 to .70. On high risk loans this range was .43 to .68. The Balanced 
Random Forest Classifier model had an accuracy score of .79, preforming much better than the first four models. Its precision on identifying low risk loans was also
high but its precision on identifying high risk loans was almost as poor as the first four models. This resulted in a recall of .91 on low risk loans and .67 on high
risk loans. The final model, the Easy Ensemble AdaBoost Classifier model, out preformed all other models with a accuracy score of .93. It had low precision identifying 
high risk loans and high precision regarding low risk loans. The recall on high risk loans was .91 while it was .94 on low risk loans. 

It is recommended that the Easy Ensemble AdaBoost Classifier model be used to predict the risk level of loans. Predicting high risk loans is the key point to modeling
this data. A business can accept or reject individual low risk loans without a serious consequence to their business.Not identifying a high risk loan can be a threat to 
a business. Unfortunately the models are not as good at predicting high risk loans as low risk loans. In this context it makes the most sense to chose the model that 
does this the best.
