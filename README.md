# evaluation-of-machine-learning-methods
Evaluation of Machine Learning Methods
******************************************************************************************************
Title: Nested Cross-Validation for Feature Selection: A Comparative Study with Nearest Neighbors

This project implements nested cross-validation for feature selection using nearest neighbors with Python 3. The goal is to automatically select the optimal feature based on 5-fold cross-validation and nested 5-fold cross-validation and then evaluate the prediction performance using both ordinary and nested 5-fold cross-validation. Finally, the project compares the C-index produced by nested 5-fold CV with the result of ordinary 5-fold CV using the best value of i (i.e., the feature providing the highest 5-fold CV C-index) and shows the difference between the two methods.
******************************************************************************************************
Title: Enhancing Metal Ion Prediction Accuracy with Leave-Replicas-Out Cross-Validation

Description:
This project focuses on predicting the total metal concentration (c_total) as well as the concentrations of Cadmium (Cd) and Lead (Pb) using K-Nearest Neighbor Regression with Euclidean distance. Different values of k (1, 3, 5, 7) are experimented with to determine the optimal parameter for the regression model.

Key Steps:

Data standardization using z-score normalization to scale the dataset features (Mod1, Mod2, Mod3).
Implementation of Leave-One-Out cross-validation and calculation of the C-index for each output (c_total, Cd, Pb).
Implementation of Leave-Replicas-Out cross-validation and calculation of the C-index for each output (c_total, Cd, Pb).
Interpretation of results, comparing the performance of both cross-validation methods and analyzing their suitability for the dataset.

Results and Interpretation:

Leave-One-Out cross-validation yielded higher C-index values compared to Leave-Replicas-Out cross-validation.
Leave-One-Out tends to be more optimistic as it predicts values based on available replicates in the training data, leading to non-realistic results. Leave-Replicas-Out is preferred for this dataset due to its ability to avoid data leakage and provide more realistic evaluations, especially considering the non-independence of the data points. 

In conclusion, Leave-Replicas-Out cross-validation demonstrates better generalization on unseen data compared to Leave-One-Out. This project showcases the importance of selecting appropriate cross-validation techniques for accurate evaluation and generalization of machine learning models, particularly in scenarios involving non-independent data.
******************************************************************************************************







