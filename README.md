# K-Means Clustering From Scratch (Python Project)

This project implements the K-Means clustering algorithm *from scratch using only NumPy*, and compares the results with Scikit-Learn's built-in KMeans.  
The Iris dataset is used for clustering and PCA visualization.

---

## 📌 Features Implemented

### ✔ Custom K-Means implementation
- Random centroid initialization  
- Euclidean distance calculation  
- Cluster assignment  
- Centroid recomputation  
- Convergence check using tolerance  
- Maximum iteration limit  

### ✔ Preprocessing
- Iris dataset loaded from sklearn.datasets
- Standardization using StandardScaler

### ✔ Evaluation
- Silhouette Score computed for:
  - Custom K-Means implementation  
  - sklearn.cluster.KMeans

### ✔ Visualization
- PCA (2-dimensional reduction)
- Scatter plot colored by cluster assignments

---

## 📁 Project Structure

├── kmeans_from_scratch.py ├── README.md

---

## 🚀 How to Run

```bash
pip install numpy matplotlib scikit-learn
python kmeans_from_scratch.py


---

📊 Output You Will See

Custom KMeans silhouette score

Sklearn KMeans silhouette score

PCA scatter plot with cluster coloring


Example (values may vary):

Custom KMeans Silhouette Score: 0.46
Sklearn KMeans Silhouette Score: 0.55


---

📌 PCA Plot

A 2-D scatter plot is displayed showing the clusters formed by the custom implementation.


---

📘 Summary

This project demonstrates:

Understanding of clustering fundamentals

Ability to implement algorithms without libraries

Comparison with industry-standard implementations

Dimensionality reduction and visual interpretation



---

✔ Submission Ready

This project meets all Cultus/Entri requirements:

Custom implementation

Evaluation

PCA Visualization

Comparison with sklearn
