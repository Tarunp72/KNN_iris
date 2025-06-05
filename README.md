# KNN_iris

# 🌸 Iris Dataset Classification using K-Nearest Neighbors (KNN)

This project demonstrates how to use the K-Nearest Neighbors algorithm to classify species in the Iris flower dataset. It includes data visualization, preprocessing, model training, and evaluation.

---

## 📁 Project Structure

- `iris_knn.ipynb` – Jupyter Notebook with complete implementation  
- `README.md` – Project description and usage guide

---

## 📊 Dataset Overview

- **Source:** `sklearn.datasets.load_iris()`
- **Classes:** `Setosa`, `Versicolor`, `Virginica`
- **Features:**
  - `sepal length (cm)`
  - `sepal width (cm)`
  - `petal length (cm)`
  - `petal width (cm)`

---

## 🎯 Objective

To build a KNN classifier that can predict the species of an Iris flower based on its sepal and petal measurements.

---

## 🧪 Workflow Summary

### 📥 1. Data Loading
- Load the Iris dataset using `sklearn.datasets.load_iris()`

### 📊 2. Data Visualization
- Convert data into a pandas DataFrame
- Plot feature distributions with seaborn:
  ```python
  sns.pairplot(df, hue='target_name', diag_kind='kde')

## 🧹 3. Preprocessing
- Split data into training and testing sets
- Apply feature scaling with `StandardScaler`

## 🧠 4. Model Training
- Use `KNeighborsClassifier(n_neighbors=5)` from scikit-learn
- Fit the model on the training data

## 📈 5. Evaluation
- Predict test labels
- Evaluate using:
  - Confusion Matrix
  - Classification Report
