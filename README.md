# Credit_Risk_Analysis

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample,undersample and combine over-undersample the data and determine which method provides the best results for logistic regression. Next, we'll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, we'll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Summary

### Naive Random Oversampling

![image](https://user-images.githubusercontent.com/100053788/177453992-93f4fecb-8f3f-4e15-81fd-89e2f6a4b9a8.png)

  a. Since the test set has higher number of low risk loan, precision will be an incorrect measure to assess validity of the machine learning algorithm.
  
  b. Precision and F1-Score for low risk loans is 1 and 0.81 respectively
  
  c. Recall for both high risk and low risk loans is 0.68
  
  d. The balanced accuracy is seen as 0.6782
  
### SMOTE Oversampling

![image](https://user-images.githubusercontent.com/100053788/177453918-b18721e5-7ae5-40d3-89da-ec5306d813ac.png)

  a. Since the test set has higher number of low risk loan, precision will be an incorrect measure to assess validity of the machine learning algorithm.
  
  b. Precision and F1-Score for low risk loans is 1 and 0.82 respectively
  
  c. Recall (positive class predictions) is lower for high risk loans 0.59 and higher for low risk loans is 0.69
  
  d. The balanced accuracy is seen as 0.6398
  
### Undersampling - Cluster Centroids

![image](https://user-images.githubusercontent.com/100053788/177453854-38f762b4-a38f-4257-ae6c-5d18f9324ee5.png)

  a. Since the test set has higher number of low risk loan, precision will be an incorrect measure to assess validity of the machine learning algorithm.
  
  b. Precision and F1-Score for low risk loans is 1 and 0.61 respectively
  
  c. Recall (positive class predictions) is higher for high risk loans 0.57 and lower for low risk loans is 0.44
  
  d. The balanced accuracy is seen as 0.5063

### SMOOTEN - Over and Under Sampling

![image](https://user-images.githubusercontent.com/100053788/177454322-4287c5a5-4eca-4bea-bd7e-dfadeb5d3016.png)

  a. Since the test set has higher number of low risk loan, precision will be an incorrect measure to assess validity of the machine learning algorithm.
  
  b. Precision and F1-Score for low risk loans is 1 and 0.73 respectively
  
  c. Recall (positive class predictions) is higher for high risk loans 0.75 and lower for low risk loans is 0.58
  
  d. The balanced accuracy is seen as 0.6613
  
 ### Balanced Random Forest Classifier
 
 ![image](https://user-images.githubusercontent.com/100053788/177454897-68d42839-6514-4ad3-a45f-0c2a3102a46a.png)

  a. Since the test set has higher number of low risk loan, precision will be an incorrect measure to assess validity of the machine learning algorithm.
  
  b. Precision and F1-Score for low risk loans is 1 and 0.95 respectively
  
  c. Recall (positive class predictions) is lower for high risk loans 0.67 and higher for low risk loans is 0.91
  
  d. The balanced accuracy is seen as 0.7877
  
  ### Easy Ensemble AdaBoost Classifier
  
  ![image](https://user-images.githubusercontent.com/100053788/177455269-13f65674-48d3-4890-aeca-7d1aea108260.png)

  a. Since the test set has higher number of low risk loan, precision will be an incorrect measure to assess validity of the machine learning algorithm.
  
  b. Precision and F1-Score for low risk loans is 1 and 0.96 respectively
  
  c. Recall (positive class predictions) is lower for high risk loans 0.90 and higher for low risk loans is 0.92
  
  d. The balanced accuracy is seen as 0.9105
  
## Summary
  
1. The undersampling models have a higher rate positive predictions for high risk loan results while the overall accuracy is lower.

2. The best classifier is the Easy Ensemble ADABoost classifier with a balanced accuracy of .9105

3. As stated in the module, using ensemble learners provide better results as they are stronger classifiers.

4. Modifying the dataset may produce better results in logistic Regression. We can also try SVM classifier.
