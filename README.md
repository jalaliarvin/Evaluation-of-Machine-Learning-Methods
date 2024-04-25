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
Title: Exploring Water Permeability Patterns in Forestry: Spatial Leave-One-Out Cross-Validation Approach

Description:

This project focuses on predicting water permeability in forestry using a K-nearest neighbor regression model (15NN) with spatial leave-one-out cross-validation. The objective is to understand how prediction performance changes with increasing geographical distance between known and unknown data points. Three data files are provided: input.csv (predictor features), output.csv (water permeability values), and coordinates.csv (geographical coordinates). Tasks include standardizing predictor features, conducting spatial leave-one-out cross-validation with 15NN, and estimating prediction performance across various distance parameters. Results show that as prediction distance increases, the C-index performance metric decreases, indicating enhanced reliability in prediction performance due to the removal of nearby data points during spatial cross-validation. This underscores the importance of spatial analysis in achieving robust and reliable predictions in forestry applications.

Tasks:

Z-score standardize the predictor features.
Perform spatial leave-one-out cross-validation with a 15NN model, estimating water permeability prediction performance across various distance parameter values (0m to 250m in 10-meter intervals).
Visualize the results by plotting the C-index (y-axis) against the distance parameter value (x-axis) in a Jupyter Notebook.

Conclusion:

Increasing prediction distance leads to a decrease in C-index performance metric, reflecting a more reliable and robust prediction performance. This occurs as nearby data points are omitted from training data during spatial cross-validation, resulting in less optimistic results and enhanced reliability. Consequently, as the hyperparameter distance increases, more nearby data points are excluded from training data, logically leading to decreased C-index performance, yet more dependable predictions. In summary, prediction performance becomes more robust and reliable as prediction distance increases.
******************************************************************************************************






