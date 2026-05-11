# Project Summary: WEKA Machine Learning Classification

## Project Description
This project uses WEKA Explorer to perform machine learning classification on structured datasets. The main experiment applies the SMO classifier to the Iris dataset and evaluates performance using both 66% Percentage Split and 10-fold Cross-validation. A second workflow uses Naive Bayes on the Play Tennis dataset to demonstrate probabilistic classification.

## Iris Dataset Analysis
The Iris dataset contains 150 flower instances across three classes: setosa, versicolor, and virginica. Each instance has four numeric predictor attributes: sepal length, sepal width, petal length, and petal width.

### Attribute Observations
- Sepal length shows some separation but also overlap across classes.
- Sepal width has substantial overlap and is less useful alone.
- Petal length clearly separates setosa and helps distinguish other classes.
- Petal width is one of the strongest separating features.

## SMO Results
### 66% Percentage Split
The model correctly classified 49 out of 51 test instances, achieving 96.0784% accuracy. Two virginica instances were misclassified as versicolor.

### 10-fold Cross-validation
The model correctly classified 144 out of 150 instances, achieving 96% accuracy. All setosa instances were classified correctly. The main confusion occurred between versicolor and virginica.

## Conclusion
The SMO classifier performed very well on the Iris dataset. The strong separation of setosa contributed to high accuracy, while the overlap between versicolor and virginica caused most of the errors. The experiment demonstrates how WEKA can be used for model training, evaluation, and interpretation without writing code.
