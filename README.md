# K-Nearest Neighbors (KNN) Classification from Scratch

This project implements the K-Nearest Neighbors (KNN) classification algorithm from scratch using only NumPy.  
The implementation is compared against Scikit-Learn’s KNeighborsClassifier for multiple values of K.  
A synthetic binary classification dataset is generated using sklearn.datasets.make_classification as required.

---

## 1. Dataset Description

A synthetic dataset is created with the following parameters:

- 500 samples  
- 10 numerical features  
- 5 informative features  
- 2 classes  
- Train-test split: 70% training, 30% testing  

This satisfies the project requirement of generating a binary classification dataset.

---

## 2. Custom KNN Implementation

The custom implementation includes:

- Euclidean distance calculation  
- Retrieval of the K nearest neighbors  
- Majority voting for classification  
- Predictions for K = 3, 5, and 7  

No external libraries are used for the KNN logic.

---

## 3. Evaluation Procedure

The following steps were performed:

1. Train the custom KNN model on training data  
2. Predict on test data  
3. Compute accuracy for K = 3, 5, and 7  
4. Repeat the same with Scikit-Learn KNeighborsClassifier  
5. Compare accuracy values for both implementations  

---

## 4. Results Summary

Accuracy values are printed in the terminal as:


Custom KNN Accuracies:
K=3: <value>
K=5: <value>
K=7: <value>

Sklearn KNN Accuracies:
K=3: <value>
K=5: <value>
K=7: <value>


The exact values depend on runtime but generally both implementations follow the same trend.

---

## 5. How to Run

Install required libraries:


pip install numpy scikit-learn


Run the program:


python knn_from_scratch.py


This generates all required outputs.

---

## 6. Deliverables Included

- Python script implementing KNN from scratch  
- Evaluation of K = 3, 5, 7  
- Comparison with Scikit-Learn  
- Synthetic binary dataset generation  
- Accuracy metrics  

All required tasks and deliverables are addressed.
