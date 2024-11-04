# Decision Tree Projects


This repository contains four different decision tree projects that utilize various datasets to showcase the power of decision trees for classification tasks. Each project includes data preprocessing, model training, evaluation, and visualization.

## Table of Contents
1. [Iris Flower Classification](#1-iris-flower-classification)
2. [Diabetes Prediction](#2-diabetes-prediction)
3. [Breast Cancer Detection](#3-breast-cancer-detection)
4. [Titanic Survival Prediction](#4-titanic-survival-prediction)

## 1. Iris Flower Classification
**Overview**: Classifies Iris flower species (setosa, versicolor, and virginica) based on sepal and petal measurements.

### Key Points
- **Dataset**: Iris dataset from scikit-learn.
- **Features**: Sepal length, sepal width, petal length, petal width.
- **Model**: Decision Tree Classifier (`max_depth=3`).
- **Visualization**: Tree shows decision splits based on petal length, separating setosa effectively.

## 1. Iris Flower Classification
**Overview**: This project classifies Iris flower species (setosa, versicolor, and virginica) using sepal and petal measurements with a decision tree model.

### Key Points
- **Dataset**: Iris dataset from scikit-learn.
- **Features Used**: Sepal length, sepal width, petal length, and petal width.
- **Model**: Decision Tree Classifier (`max_depth=3`).
- **Visualization**: The decision tree visual clearly shows how the model splits data based on petal and sepal measurements.

### Results
- **Model Accuracy**: The decision tree achieved a perfect accuracy of **100%** on the test set (`clf.score(test_x, test_lab) = 1.0`), indicating it classified all test samples correctly.
- **Decision Tree Visualization**:
  - The first split is based on `petal length (cm) <= 2.45`, effectively separating setosa from the other species.
  - Subsequent splits are based on `petal length` and `petal width`, further distinguishing between versicolor and virginica.

![Decision Tree Visualization](https://github.com/user-attachments/assets/40054b3f-82a9-40d3-b163-d702cf171a0a)


### Interpretation
- The decision tree indicates that `petal length` is the most significant feature for the first level of classification.
- Gini impurity and sample distributions at each node help interpret the purity of splits, with terminal nodes (leaves) showing pure classifications (Gini = 0).

### Code Reference
Refer to the Python script or Jupyter notebook in the repository for full code details, including data loading, preprocessing, model training, and visualization.



---

## 2. Diabetes Prediction
**Overview**: Predicts diabetes presence using the Pima Indians Diabetes dataset.

### Key Points
- **Dataset**: Pima Indians Diabetes dataset.
- **Features**: Pregnancies, Glucose, Blood Pressure, BMI, Age, etc.
- **Model**: Decision Tree Classifier with Gini and entropy criteria.
- **Optimization**: Criterion set to `"entropy"` with `max_depth=3` for better performance.

### Results
- Initial model accuracy: **67.5%**.
- Optimized model accuracy: **77.1%**.

---

## 3. Breast Cancer Detection
**Overview**: Classifies breast cancer samples as malignant or benign based on cell nuclei features.

### Key Points
- **Dataset**: Breast Cancer dataset from scikit-learn.
- **Features**: 30 features related to cell nuclei.
- **Model**: Decision Tree Classifier (criterion: entropy).
- **Visualization**: Highlights splits using significant features like mean area and concave points.

### Results
- Achieved **X%** accuracy on the test set.
- Tree visualization helps interpret feature importance and decision paths.

---

## 4. Titanic Survival Prediction
**Overview**: Predicts passenger survival based on select features from the Titanic dataset.

### Key Points
- **Dataset**: Titanic dataset from Kaggle.
- **Features**: Pclass, Sex, Age, Fare.
- **Preprocessing**: Categorical data mapping and handling missing values.
- **Model**: Decision Tree Classifier.
- **Visualization**: Displays decision rules and important nodes based on passenger attributes.

### Results
- Model accuracy: **X%** on the test set.
- Visualization reveals key features impacting survival predictions (e.g., `Sex` and `Age`).

---

## Getting Started
Clone this repository to explore and run each project:
```bash
git clone https://github.com/yourusername/decision-tree-projects.git
cd decision-tree-projects
