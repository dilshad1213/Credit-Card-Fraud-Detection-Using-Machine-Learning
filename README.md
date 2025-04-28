# Machine-Learning
# 2.3 Supervised Machine Learning Algorithms
This section discusses several commonly used supervised learning models including Logistic Regression, k-Nearest Neighbors, Support Vector Machines, Decision Trees, Gaussian Naive Bayes, Random Forest, Gradient Boosting, and Linear Discriminant Analysis.
# 2.3.1 Logistic Regression (LR)
Logistic Regression is a classification method under supervised learning that operates by extracting numerical features from inputs, assigning weights to each, and passing the weighted sum through a sigmoid function. This transformation generates a probability score, and a threshold is applied to classify the data. Unlike linear regression, logistic regression maps outcomes to a range between 0 and 1 using the logistic function:
                                𝐿𝑜𝑔𝑖𝑠𝑡𝑖𝑐(𝜂)=1/1+(𝑒^-𝜂)
As the input η ranges from negative to positive infinity, the function compresses it into the interval [0, 1]. In our implementation, we used up to 4000 iterations to ensure convergence.
# 2.3.2 k-Nearest Neighbors (KNN)
KNN is a non-parametric technique employed to classify diabetic-related data. The algorithm assigns labels based on the majority vote among the closest K data points, where proximity is determined by a chosen distance metric. For example, with K set to 1, a data point is categorized the same as its nearest neighbor. Below is a simplified outline of the KNN method:

KNN Steps:

Store training examples in an array.

Calculate the distance between each training sample and the new point.

Identify the K smallest distances.

Return the most common label among these K neighbors.

# 2.3.3 Support Vector Machine (SVM)
Support Vector Machines define a boundary, known as a hyperplane, that best separates the data into classes. For linearly separable data, this is a straight line or plane, but SVM can also handle non-linear data via kernel functions.

The objective is to maximize the margin between classes, influenced by the regularization parameter which balances training accuracy and model complexity.
