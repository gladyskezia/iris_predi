# Logistic Regression from Scratch (NumPy Implementation)

This project implements a binary logistic regression classifier using only NumPy.  
The goal is to demonstrate a clear understanding of the mathematical foundations of logistic regression, including the sigmoid function, binary cross-entropy loss, gradient descent optimization, and manual evaluation metrics.  
No Scikit-Learn model classes or metric functions were used in the core implementation.

---

## 1. Dataset Generation

A synthetic two-dimensional binary classification dataset was generated using `make_classification`.  
The dataset characteristics are:

- 500 samples  
- 2 informative features  
- No redundant features  
- Two class labels (0 and 1)  
- One cluster per class  
- A fixed random seed for reproducibility  

The dataset is suitable for visualizing the decision boundary in a two-dimensional feature space.

The dataset was divided into training and testing splits using a 70%/30% ratio.

---

## 2. Logistic Regression Implementation

The logistic regression model was developed entirely using NumPy.  
The following components were implemented:

### 2.1 Sigmoid Function
The sigmoid mapping function is defined as:

*s(z) = 1 / (1 + exp(−z))*

This converts linear model outputs into probabilities between 0 and 1.

### 2.2 Model Hypothesis
Given input features *X*, weights *w*, and bias *b*, the hypothesis is:

*h(x) = sigmoid(w · x + b)*

### 2.3 Loss Function (Binary Cross-Entropy)
The loss function used during optimization is:

*J(w, b) = −(1/m) Σ [ y log(h) + (1−y) log(1−h) ]*

### 2.4 Gradient Descent
Gradients for weights and bias were computed using:

*dw = (1/m) Xᵀ(h − y)*  
*db = (1/m) Σ(h − y)*

Model parameters were updated iteratively for a fixed number of iterations, using a learning rate of 0.1.

### 2.5 Prediction Rule
Predictions were assigned using a threshold of 0.5:

- If probability ≥ 0.5 → class 1  
- Otherwise → class 0  

---

## 3. Evaluation Metrics (Manual NumPy Calculations)

The evaluation did not use Scikit-Learn metrics.  
Instead, all metrics were computed manually using NumPy.

### 3.1 Accuracy  
Accuracy was computed as the proportion of correct predictions.

### 3.2 Precision  
Precision was computed using:

- True Positives (TP): predicted 1 and actual 1  
- Predicted Positives (PP): predicted 1  

*precision = TP / PP*

### 3.3 Recall  
Recall was computed using:

- Actual Positives (AP): actual value 1  

*recall = TP / AP*

These metrics provide an objective assessment of the model’s classification performance.

---

## 4. Learned Parameters

After gradient descent training, the model outputs the final learned:

- Weight vector (length 2)  
- Bias value  

These values are printed when the script is executed.  
They represent the linear decision boundary fitted to the dataset.

---

## 5. Decision Boundary Visualization

A contour plot was generated using model predictions across a dense mesh grid covering the feature space.  
The generated plot:

- Displays the separating boundary created by the logistic regression model  
- Shows how the model partitions the space between the two classes  
- Overlays the dataset points colored by their true labels  

The plot is saved as:

```
decision_boundary.png
```

This satisfies the requirement for visualizing the learned classifier.

---

## 6. How to Run the Project

Install required libraries:

```
pip install numpy scikit-learn matplotlib
```

Execute the source code:

```
python logistic_regression_from_scratch.py
```

This will:

1. Generate the dataset  
2. Train the logistic regression model  
3. Compute accuracy, precision, and recall  
4. Print the final weights and bias  
5. Save `decision_boundary.png`  

---

## 7. Deliverables Completed

This submission includes:

- A complete Python implementation of logistic regression from scratch  
- Manual computations for accuracy, precision, and recall  
- A decision boundary visualization image  
- A detailed explanation of methodology, model components, and evaluation  

All required tasks and deliverables described in the assignment instructions have been addressed.
