# Credit Risk Analysis

The purpose of this project is to implement different techniques to train and evaluate machine learning models with unbalanced classes using resampling. For this project I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm, then implemented a combinatorial approach of over-and undersampling using the SMOTEENN algorithm. Finally, in order to predict credit risk, I implemented the BalancedRandomForestClassifier and EasyEnsembleClassifier.


---


## Results


* Describe the balanced accuaracy score and the precision and recall scores of all six machine learning models:

### 1.- Naive Random Oversampling

![1 - Naive Random](https://user-images.githubusercontent.com/113866707/217706569-425c475c-47a7-458b-abf9-5c8c68defa36.png)

* Balanced Accuracy Score of 64%. We can conclude that this model works 64 out of 100 times it is run.
* Precision score of this model is not good for identifying high-risk loans as shown in the Classification Report Imbalanced, where 0.01 high-risk credits were identified.
* Recall of 61% for high risk and 68% for low risk.

### 2.- SMOTE Oversampling

![2 - SMOTE](https://user-images.githubusercontent.com/113866707/217706589-9230fc07-ea71-4c74-aa09-4bd76e5a337e.png)

* Balanced Accuracy Score of 62%. We can conclude that this model works 62 out of 100 times it is run.
* Precision score of this model is not good for identifying high-risk loans as shown in the Classification Report Imbalanced, where 0.01 high-risk credits were identified.
* Recall of 61% for high risk and 64% for low risk.

### 3.- Undersampling


![Captura de pantalla 2023-02-09 a la(s) 22 46 11](https://user-images.githubusercontent.com/113866707/218003198-16a63082-a324-43d1-97de-90681063152d.png)

* Balanced Accuracy Score of 52%. We can conclude that this model works 52 out of 100 times it is run.
* Precision score of this model is not good for identifying high-risk loans as shown in the Classification Report Imbalanced, where 0.01 high-risk credits were identified.
* Recall of 61% for high risk and 43% for low risk.

### 4.- Combination (Over and Under) Sampling

![4 - Combination](https://user-images.githubusercontent.com/113866707/217706625-4c011df6-5e01-4d50-8f86-e3c8d0b4e754.png)

* Balanced Accuracy Score of 65%. We can conclude that this model works 65 out of 100 times it is run.
* Precision score of this model is not good for identifying high-risk loans as shown in the Classification Report Imbalanced, where 0.01 high-risk credits were identified.
* Recall of 69% for high risk and 62% for low risk.

### 5.- Balanced Random Forest Classifier

![5 - BRF](https://user-images.githubusercontent.com/113866707/217706641-9ce2f679-eda8-40b4-9509-ff3ec4e98429.png)

* Balanced Accuracy Score of 78%. We can conclude that this model works 78 out of 100 times it is run.
* Precision score of this model is not good for identifying high-risk loans as shown in the Classification Report Imbalanced, where 0.04 high-risk credits were identified.
* Recall of 67% for high risk and 91% for low risk.

### 6.- Easy Ensemble AdaBoost Classifier

![6 - AdaBoost](https://user-images.githubusercontent.com/113866707/217706656-99cd0858-75f5-4c00-a345-ae46ab1ff102.png)

* Balanced Accuracy Score of 92%. We can conclude that this model works 92 out of 100 times it is run.
* Precision score of this model is not good for identifying high-risk loans as shown in the Classification Report Imbalanced, where 0.07 high-risk credits were identified.
* Recall of 91% for high risk and 94% for low risk.


---

## Summary

* Each model adjusts the data accordingly to the machine learning model algorithm. As we can see, each particular model has it's own accuracy score. For this exercise the best ranked model was the AdaBoost model with 92% accuracy, also, this model is able to classify better for high and low risk credits. In order to enhance the classification of risk levels, it will be needed to analyze the current data and identify why high risk loans tend to be difficult to classify on each model.




