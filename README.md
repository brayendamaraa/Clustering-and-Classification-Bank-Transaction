# Clustering and Classification of Bank Transactions

This project explores **unsupervised and supervised machine learning techniques** to analyze bank transaction data. The goal is to **cluster modified transaction data using K-Means** and then **classify the resulting clusters using Decision Tree and Random Forest models**, comparing their performance.

The dataset used comes from the Kaggle dataset **“Bank Transaction Dataset for Fraud Detection.”**

---

## Project Overview

Financial transaction datasets contain patterns that can reveal customer behavior or potential fraud. Clustering techniques such as **K-Means** group similar transactions based on their features, enabling pattern discovery without labeled data.

After clustering, supervised models such as **Decision Tree** and **Random Forest** can be trained to **predict cluster membership**, allowing efficient classification of new transactions.

This project demonstrates a pipeline combining:

1. **Data preprocessing and feature engineering**
2. **Unsupervised clustering using K-Means**
3. **Supervised classification using Decision Tree and Random Forest**
4. **Performance comparison between the models**

---

# Dataset

Dataset source:  
**Bank Transaction Dataset for Fraud Detection (Kaggle)**

The dataset contains simulated banking transaction records with features such as:

- Transaction amount
- Account balance
- Transaction duration
- Customer attributes
- Transaction metadata

These features allow the detection of behavioral patterns or anomalies in transaction activity.

---

# Methodology

The project workflow consists of several stages.

## 1. Data Preprocessing

The raw dataset is modified and prepared for modeling:

- Handling missing values
- Encoding categorical variables
- Feature selection and transformation
- Data normalization or scaling

These steps ensure that the dataset is suitable for clustering and classification models.

---

## 2. Clustering with K-Means

K-Means clustering groups transactions into clusters based on similarity between data points.

The algorithm works by:

1. Randomly selecting **k centroids**
2. Assigning each data point to the nearest centroid
3. Updating centroids based on the mean of each cluster
4. Repeating until cluster assignments stabilize

The optimal number of clusters is determined using the **Elbow Method**.

---

## 3. Classification Models

After clustering, cluster labels are used as targets for supervised learning.

Two models are trained and compared:

### Decision Tree

A Decision Tree is a tree-based model that splits data based on feature thresholds to classify observations.

Advantages:

- Easy to interpret
- Handles non-linear relationships
- Requires minimal data preprocessing

---

### Random Forest

Random Forest is an ensemble learning method that combines multiple decision trees.

Advantages:

- Higher accuracy
- Reduced overfitting
- Better generalization

---

## 4. Model Evaluation

Both classification models are evaluated using common metrics such as:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

The results are then compared to determine which model performs better at predicting cluster membership.

---

# Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook
