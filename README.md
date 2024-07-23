# Machine-Learning

## 50.007 Machine Learning - Summer 2024
Project Summary
Online hate speech is an important issue that breaks the cohesiveness of online social communities and even raises public safety concerns in our societies. Motivated by this rising issue, researchers have developed many traditional machine learning and deep learning methods to detect hate speech on online social platforms automatically.

Essentially, the detection of online hate speech can be formulated as a text classification task: "Given a social media post, classify if the post is hateful or non-hateful". In this project, you are to apply machine learning approaches to perform hate speech classification. Specifically, you will need to perform the following tasks.

### Task 1: Implement Logistics Regression
Implement a Logistic Regression model from scratch. Note that you are NOT TO USE the sklearn logistic regression package or any other pre-defined logistic regression package for this task!

### Key Task Deliverables
1a. Code implementation of the Logistic Regression model.
1b. Prediction made by the Logistic Regression model on the Test set.

### Functions:
-- sigmoid(z): A function that takes in a Real Number input and returns an output value between 0 and 1.
-- loss(y, y_hat): A loss function that allows us to minimize and determine the optimal parameters. The function takes in the actual labels y and the predicted labels y_hat, and returns the overall training loss. 
-- gradients(X, y, y_hat): The Gradient Descent Algorithm to find the optimal values of our parameters. The function takes in the training feature X, actual labels y and the predicted labels y_hat, and returns the partial derivative of the Loss function with respect to weights (w) and bias (db).
-- train(X, y, bs, epochs, lr): The training function for your model.
-- predict(X): The prediction function to apply validation and test sets.

### Task 2: Apply dimension reduction techniques
Dimension reduction is the transformation of data from a high-dimensional space into a low-dimensional space so that the low-dimensional representation retains some meaningful properties of the original data. The train dataset contains 5000 TD-IDF features. Apply PCA to reduce the dimension of features.

### Key Task Deliverables
2a. Code implementation of PCA on the train and test sets. Note that you are allowed to use the sklearn package for this task.
2b. Report the Macro F1 scores for applying 2000, 1000, 500, and 100 components on the test set. Note that you will have to submit your predicted labels to Kaggle to retrieve the Macro F1 scores for the test set and report the results in your final report. Use KNN as the machine learning model for your training and prediction (You are also allowed to use the sklearn package for KNN implementation) (set n_neighbors=2).
