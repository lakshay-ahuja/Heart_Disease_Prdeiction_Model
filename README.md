# Heart_Disease_Prdeiction_Model
# INTRO:
I found this Cleveland Clinic Heart Disease Dataset on Kaggle. 

The data consists of 14 attributes. Some attributes are continuous, like age and cholesterol level. Some are categorical, like sex and type of chest pain. The task is to use the first 13 attributes to predict the 14th - the presence of heart disease in a patient. This task is complicated by the fact that the training set is so small.

In this project I'll explore various ML models for this task. My main tools will be the python scikit-learn and tensorflow libraries. I found that most models achieve an accuracy of .885. This consistency across many types of model suggests a Bayes Error probably around 8-10%.
# Steps:
1. Import modules and datset.
2. Rename data fields to be more descriptive.
3. Use one-hot encoding for categorical variables.
4. Split the data into training and testing sets.
5. Use Scikit-Learn Models: Logistic Regression, K Neighbours Classifier, SVM(Support Vector Machine), Naive Bayes, Decision Tree and Random Forest. Each of these models has a fit() method, as well as predict() and score(). This uniformity will allow us to make an ensemble voting classifier.
6. Make a simple Deep Learning Model with three fully-connected layers of 100 units, 100 units, 10 units, and ReLU activations. This last layer feeds into a single unit with sigmoid activation.
7. Train the model and try it on test data set.
8. Make a Voting Ensemble containing all the scikit-learn models(7) and set the threshold for votes accordingly. Check its perfomance.
