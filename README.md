# Breast-Cancer-Classification-using-K-Nearest-Neighbors

## Objective

The objective of this project is to develop a Machine Learning model using the K-Nearest Neighbors (KNN) algorithm to classify breast tumors as **Malignant (M)** or **Benign (B)** based on diagnostic measurements. The project demonstrates data preprocessing, feature scaling, model training, and performance evaluation using standard classification metrics.

---

## Dataset

**Dataset Name:** Breast Cancer Wisconsin Diagnostic Dataset

**Kaggle Link:**
https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data

**Target Variable:**
- `diagnosis`
  - M = Malignant
  - B = Benign

---

## Libraries Used

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Methodology

1. Loaded the dataset using Pandas.
2. Displayed the first five records.
3. Identified numerical features and the target variable.
4. Examined dataset information and summary statistics.
5. Checked for missing values.
6. Removed unnecessary columns (`id` and `Unnamed: 32`).
7. Encoded the target variable using LabelEncoder.
8. Standardized all feature values using StandardScaler.
9. Split the dataset into 80% training and 20% testing sets.
10. Trained a K-Nearest Neighbors (KNN) classifier with **K = 5**.
11. Predicted the class labels for the test dataset.
12. Evaluated the model using Accuracy, Precision, Recall, F1-Score, and Confusion Matrix.

---

## Results

The KNN classifier achieved excellent classification performance on the Breast Cancer Wisconsin Diagnostic dataset. The evaluation metrics showed high accuracy along with strong precision, recall, and F1-score, indicating that the model can effectively distinguish between malignant and benign tumors. The confusion matrix also demonstrated that only a small number of samples were misclassified.

---

## Observations

1. The KNN classifier achieved high accuracy in distinguishing malignant and benign tumors.

2. Precision and recall values indicate that the model performs well in identifying malignant cases while minimizing false predictions.

3. Feature scaling significantly improved the performance because KNN relies on distance calculations between data points.

---

## Conclusion

In this assignment, a K-Nearest Neighbors (KNN) classifier was developed to classify breast tumors as malignant or benign using the Breast Cancer Wisconsin Diagnostic dataset. After preprocessing the data by removing unnecessary columns, encoding the target variable, and standardizing the features, the KNN model achieved high classification performance. The evaluation metrics, including accuracy, precision, recall, and F1-score, demonstrated that the model effectively distinguished between the two classes. Feature scaling played a crucial role because KNN calculates distances between data points, and unscaled features can disproportionately influence the results. One limitation of KNN is that its prediction time increases with larger datasets, making it computationally expensive for large-scale applications.
