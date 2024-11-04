![image](https://github.com/user-attachments/assets/694dc2bb-139a-4f58-bb35-4c313bd12a6d)# Decision Tree Projects


This repository contains four different decision tree projects that utilize various datasets to showcase the power of decision trees for classification tasks. Each project includes data preprocessing, model training, evaluation, and visualization.

## Table of Contents
1. [Iris Flower Classification](#1-iris-flower-classification)
2. [Diabetes Prediction](#2-diabetes-prediction)
3. [Breast Cancer Detection](#3-breast-cancer-detection)
4. [Titanic Survival Prediction](#4-titanic-survival-prediction)



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
**Overview**: This project aims to predict the presence of diabetes using the Pima Indians Diabetes dataset by training and evaluating a decision tree classifier.

### Key Points
- **Dataset**: Pima Indians Diabetes dataset.
- **Features Used**: Pregnancies, Glucose, Blood Pressure, Skin Thickness, Insulin, BMI, Diabetes Pedigree Function, Age.
- **Model**:
  - Initial Decision Tree Classifier with default parameters achieved an accuracy of **67.53%**.
  - Optimized Decision Tree Classifier with `criterion="entropy"` and `max_depth=3` achieved an improved accuracy of **77.06%**.
- **Data Balance**: The dataset has an imbalance in outcomes, as shown by the bar plot of outcome counts.

### Results
- **Initial Model Accuracy**: **67.53%** on the test set with default parameters.
- **Optimized Model Accuracy**: **77.06%** on the test set using the entropy criterion and a max depth of 3, demonstrating significant improvement.

### Decision Tree Visualization
- The decision tree split on key features such as `Glucose` and `BMI`, highlighting their importance in predicting diabetes.


![Decision Tree Visualization](https://github.com/user-attachments/assets/c083f095-5e5b-44a3-b9b1-d4e03c25de94)

### Data Distribution Plot
- The plot below shows the distribution of outcomes (0: non-diabetic, 1: diabetic), which indicates the class imbalance in the dataset.

![Outcome Count Plot](https://github.com/user-attachments/assets/fd90fd6e-de0e-4815-b0dc-eaef3a80149b)


### Interpretation
- The decision tree reveals that `Glucose` and `BMI` are critical features in diabetes diagnosis.
- The improvement in accuracy when using `criterion="entropy"` and limiting tree depth helps reduce overfitting and enhances generalizability.

### Code Reference
Refer to the project code for detailed steps on data preparation, training, and evaluation, including the creation of visualizations.




---

## 3. Breast Cancer Detection
**Overview**: This project uses a decision tree classifier to classify breast cancer samples as malignant or benign based on features related to cell nuclei.

### Key Points
- **Dataset**: Breast Cancer dataset from scikit-learn.
- **Features Used**: Mean area, mean texture, mean smoothness, mean symmetry, mean concave points, etc.
- **Model**: Decision Tree Classifier (`criterion="entropy"`).

### Results
- **Training Data Accuracy**: **100%**, indicating the model perfectly classifies training samples.
- **Test Data Accuracy**: **97.08%**, showing that the model generalizes well and performs accurately on unseen data.

### Decision Tree Visualization
- The decision tree splits based on significant features such as `mean area` and `mean concave points`, highlighting their importance in the classification process.


![Decision Tree Visualization](https://github.com/user-attachments/assets/9bcb7b34-ac0d-43f6-a8de-fa65988b61f8)

### Interpretation
- The decision tree model shows high accuracy on both training and test data, indicating effective learning with minimal overfitting.
- The use of the `entropy` criterion emphasizes the most informative feature splits, leading to deeper insights into feature importance.

### Code Reference
Refer to the project code for data loading, model training, and evaluation steps, along with the visualization generation.


---
## 4. Titanic Survival Prediction
**Overview**: This project predicts passenger survival based on selected features from the Titanic dataset using a decision tree classifier.

### Key Points
- **Dataset**: Titanic dataset.
- **Features Used**: Sex, Age, Pclass, Fare, etc.
- **Model**: Decision Tree Classifier trained with default settings.

### Results
- **Test Data Accuracy**: The model achieved an accuracy of **74.86%** on the test set, demonstrating a fair performance in classifying passenger survival.
- **Decision Tree Visualization**:
  - The tree splits on key features like `Sex`, `Age`, and `Pclass`, showing their importance in predicting survival.


![Decision Tree Visualization](https://github.com/user-attachments/assets/65e6ad37-0291-472a-a13a-5f3649bbf68a)

### Interpretation
- The decision tree indicates that `Sex` is a primary factor in determining survival, followed by age and passenger class (`Pclass`).
- The visualization of the tree helps explain the model's decision-making process, highlighting the most significant features.

### Data Distribution
- The dataset's distribution can be examined to understand the balance of features and outcomes.

### Code Reference
Check the project code for complete steps on data preprocessing, model training, evaluation, and generating the tree visualization.


---

## Getting Started
Clone this repository to explore and run each project:
```bash
git clone https://github.com/yourusername/decision-tree-projects.git
cd decision-tree-projects
```
### Prerequisites
- **Python Version**: Python 3.x
- **Libraries**: 
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `matplotlib`

### Contact
For any questions or feedback, please contact me via email:

**Email**: [elhmarmin@gmail.com](mailto:elhmarmin@gmail.com)

