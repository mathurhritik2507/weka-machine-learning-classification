# WEKA Machine Learning Classification

## Overview
This repository contains WEKA-based machine learning classification work using the Iris and Play Tennis datasets. The project demonstrates dataset preparation in ARFF format, classifier training, model evaluation, confusion matrix interpretation, and error visualization.

## Objective
The objective of this project is to understand how supervised machine learning models perform in WEKA Explorer and how model performance can be compared using accuracy, MAE, RMSE, Kappa statistic, and confusion matrices.

## Tools & Technologies
- WEKA Explorer
- ARFF datasets
- SMO / Support Vector Machine
- Naive Bayes
- Percentage Split evaluation
- 10-fold Cross-validation
- Confusion Matrix
- Error Visualization

## Datasets
### Iris Dataset
The Iris dataset contains 150 instances and three classes: setosa, versicolor, and virginica. It includes four numeric features: sepal length, sepal width, petal length, and petal width.

### Play Tennis Dataset
The Play Tennis dataset is a small classification dataset used to demonstrate Naive Bayes classification based on weather-related attributes such as Outlook and Wind.

## Methodology
1. Loaded ARFF datasets into WEKA Explorer.
2. Reviewed attributes and class distributions in the Preprocess tab.
3. Applied SMO classifier on the Iris dataset.
4. Evaluated SMO using 66% Percentage Split and 10-fold Cross-validation.
5. Applied Naive Bayes on the Play Tennis dataset.
6. Interpreted classifier output using accuracy, MAE, RMSE, Kappa statistic, and confusion matrix.
7. Used WEKA visualization tools to inspect classifier errors.

## Key Results
### SMO on Iris Dataset
- 66% Percentage Split: 49 correctly classified instances out of 51 test instances.
- Accuracy: 96.0784%
- Incorrectly classified instances: 2
- MAE: 0.2309
- RMSE: 0.2877
- Kappa statistic: 0.9408

### SMO with 10-fold Cross-validation
- Correctly classified instances: 144 out of 150
- Accuracy: 96%
- Incorrectly classified instances: 6
- MAE: 0.2311
- RMSE: 0.288
- Kappa statistic: 0.94

## Conclusion
The SMO classifier performed strongly on the Iris dataset, achieving approximately 96% accuracy in both evaluation methods. The setosa class was perfectly separated, while most errors occurred between versicolor and virginica because these classes overlap more closely in feature space.

## Repository Structure
```text
weka-machine-learning-classification/
├── README.md
├── data/
│   ├── iris.arff
│   └── play_tennis.arff
├── weka_outputs/
│   ├── smo_iris_66_percent_split_output.txt
│   ├── smo_iris_10_fold_cross_validation_output.txt
│   └── naive_bayes_play_tennis_output_notes.txt
├── results/
│   ├── iris_smo_results_summary.csv
│   └── confusion_matrices.csv
├── screenshots/
│   └── README.md
└── docs/
    ├── project_summary.md
    └── github_upload_checklist.md
```

## Future Improvements
- Add more WEKA classifiers such as J48, Random Forest, and Logistic Regression.
- Recreate the same experiments in Python using Scikit-learn.
- Compare WEKA results with Python model results.
- Add final screenshots from WEKA Explorer for each classifier output and error visualization.
