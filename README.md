## Spam Comment Detection using Naive Bayes Classifier

This Python code aims to detect spam comments using a Bernoulli Naive Bayes classifier. Here's a breakdown of its functionality:

### 1. Data Loading and Preprocessing
- Loads a dataset named 'Youtube01-Psy.csv' containing comment data.
- Selects only the 'CONTENT' (comment text) and 'CLASS' (spam or not spam) columns.
- Maps the numerical class labels to categorical labels: 0 for "Not Spam" and 1 for "Spam".

### 2. Text Vectorization
- Converts the comment text into numerical features using the CountVectorizer.
- Splits the dataset into feature vectors (x) and target labels (y).

### 3. Model Training
- Splits the data into training and testing sets using a 80-20 split ratio.
- Initializes a Bernoulli Naive Bayes model.
- Fits the model to the training data.

### 4. Model Evaluation
- Evaluates the trained model's performance on the testing data using the `score` method.
- Prints the accuracy score of the model on the testing set.

### 5. Predicting Spam Comments
- Takes a sample comment text.
- Vectorizes the sample using the CountVectorizer.
- Predicts whether the sample comment is spam or not.
- Prints "Spam Comment" if the prediction is 1, otherwise prints "Not Spam Comment".

### Conclusion
This code demonstrates the process of training a machine learning model to classify comments as spam or not spam using a Bernoulli Naive Bayes classifier. It also provides a simple example of using the trained model to predict the class of a new comment.
