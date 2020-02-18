# wine_quality_prediction

In this project, I have worked on predicting the quality of wine. For that I have used a variety of different models such as Logistic Regression, Logistic Regression with SMOTE, Decision Trees, Naive Bayes, Random Forest Classifier, SVM and XGB Classifier.

Let us first explore the dataset.
Info Data
![alt text]([img]https://i.imgur.com/jUfprPr.jpg)

Checking for Null Values in the columns
![alt text]([img]https://i.imgur.com/SLWEWHk.jpg)

We see that there are no null values present the columns. Let us now try to visualize and see the data distribution among various classes of quality.
After plotting the count plot for quality column with seaborn,
![alt text]([img]https://i.imgur.com/yzWwOMQ.jpg)
We can clearly observe that the data is not uniformly distributed among the different classes. Most of the wines in the dataset are of either quality 5 or 6. We have an imbalanced to deal with here.

Let us now look at the correlation matrix of features and try to understand the data more.
![alt text]([img]https://i.imgur.com/rfH3QSJ.jpg)

From correlation matrix, we can clearly infer that as the quantity of alcohol increases in the wine, it becomes more superior in terms of quality. Whereas lower the volatile acidity, the better it is. Citric Acid is also positively correlated with the quality.

After scaling the dataset and applying PCA, the accuracy achieved by various models for the given dataset are as follows:
![alt text]([img]https://i.imgur.com/q2qzSRL.jpg)

We can see that Random Forest has the highest accuracy of almost 90% followed by XGBoost Classifier 86.6 % accuracy approximately. Surprisingly the model accuracy degraded considerably after applying SMOTE (oversampling) technique with Logistic Regression.
