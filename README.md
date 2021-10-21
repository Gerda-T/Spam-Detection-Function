# Spam Detection Function
This is an implementation of a spam detector function that accepts three arguments;
- train df
- valid df
- test df
In this spam function, the first step performs text vectorization based on the tf-idf method. 
In the next step, four text classifiers on vectorized data was applied
The models includes:
- Logistic Regression Classifier
- Multinomial Naive Bayes Classifier
- Decision Tree Classifier
- Linear Support Vector Classifier
The spam detector functions returns a dictionary with the following keys;
LogistricRegression, MultinomialNB, DecisionTreeClassifier, LinearSVC with confusion matric for validation data and corresponding model;
BestClassifier-name of the classifier with the lowest number of spam messages misclassified
TfidVectorizer- matrix after the Tfidf vectorization is applied to the test DataFrame
Prediction- Predicted labels(0 or 1) for the test DataFrame using the classifier chosen as BestClassifer.
