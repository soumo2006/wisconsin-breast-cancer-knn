# Wisconsin Breast Cancer Classification using KNN

## 📌 Project Overview

This project uses the **K-Nearest Neighbors (KNN)** machine learning algorithm to classify breast cancer cases as **Malignant** or **Benign**.

The model is trained using the Wisconsin Breast Cancer dataset and uses **30 medical features** for classification.

## 📊 Dataset

**Dataset:** Wisconsin Breast Cancer Dataset

The dataset contains medical measurements related to breast tumor characteristics.

### Input

The model takes 30 medical features as input, including:

* Radius
* Texture
* Perimeter
* Area
* Smoothness
* Compactness
* Concavity
* Concave Points
* Symmetry
* Fractal Dimension

These measurements are available as mean, standard error (`se`), and worst-case values.

### Output

The model predicts one of two classes:

* **Malignant**
* **Benign**

## 🤖 Machine Learning Algorithm

**K-Nearest Neighbors (KNN)**

Different values of `K` were tested from 1 to 29. The final model uses:

```python
KNeighborsClassifier(n_neighbors=8)
```

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

1. Removed duplicate records.
2. Removed the `id` column.
3. Separated features and target variable.
4. Split the dataset into training and testing sets using an 80/20 split.
5. Applied `StandardScaler` to scale the features.
6. Applied **SMOTE** to the training data to address class imbalance.

## 📈 Model Performance

The model was evaluated on the **test dataset**.

| Metric   | Score |
| -------- | ----: |
| Accuracy |   95% |
| Recall   |   95% |
| F1 Score |   95% |

A confusion matrix was also used to evaluate the classification performance.

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Imbalanced-learn
* Jupyter Notebook / Google Colab

## 🎯 Prediction

The notebook also allows the user to enter the 30 medical features manually.

The trained KNN model then predicts:

```text
Malignant
```

or

```text
Benign
```

## 👨‍💻 Author

**Soumotirtha Das**

Built completely independently as a machine learning classification project.

