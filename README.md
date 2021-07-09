# Loan-Approval-Prediction
Customer first apply for home loan after that company validates the customer eligibility for loan. 
details are Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History and others. 
Plots were plotted for categorical variables to show whether loan was approved or not based on Gender, Marital status, number of dependents, education , employment etc.
For numerical columns, it was plotted based on applicant, co applicant income (box-whisker) no significant difference.
1.	Encoding Categorical Features.
2.	dropping missing values.

split training and test data. 

Model 1:
Decision Tree Classifier
Training Accuracy > Test Accuracy with default settings of Decision Tree classifier. Hence, model is overfit
tuning 'Max_Depth' of tree
Visulazing Decision Tree with Max Depth = 3
some of the leafs have less than 5 samples hence our classifier might overfit.
we will choose Min_Samples_leaf to 35 to improve test accuracy.
Let's use this Decision Tree classifier on unseen test data and evaluate Test Accuracy, F1 Score and Confusion Matrix 
Mis-classifications
It can be seen that majority of the misclassifications are happening because of Loan Reject applicants being classified as Accept.
Model 2: Random Forest Classifier
Random Forest gives same results as Decision Tree Classifier. Finally, we will try Logistic Regression Model by sweeping threshold values.
Model 3: Logistic Regression
Logistic Regression Confusion matrix is very similar to Decision Tree and Random Forest Classifier. In this analysis, we did extensive analysis of input data and were able to achieve Test Accuracy of 86 %
