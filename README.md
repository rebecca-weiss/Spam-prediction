# Spam-prediction
Machine learning project to predict spam emails using keywords from the spambase dataset from UCI
Dataset: https://archive.ics.uci.edu/ml/datasets/spambase



# Breakdown of workflow:
1. Load and split dataset at random into 80% training and 20% testing
2. Create a bootstrap n=1000 and vary the size of columns (p), and choose the value that results in the lowest cross-validation error 
3. After determing p # of columns, I will train a decision tree classifier on the bootstrap sample
4. Repeat these calculations to generate T ∈ {1, 50, 100, 150, 200, 300, 400} trees and evaluate on the training set.
5. Determine train and test error, F1 score, and AUC by varying T in the range {1, 50, 100, 150, 200, 300, 400}
6. Train a Random Forest algorithm with 10, 50, and 100 decision trees and report similar metrics on both the training and testing sets
7. Report/visualize the top 10 features having the most influence on the model
