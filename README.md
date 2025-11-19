# Logistic Regression from Scratch (NumPy Implementation)

This project implements a logistic regression classifier using only NumPy.  
The goal is to demonstrate a full mathematical and programmatic understanding of logistic regression, including data generation, model training, evaluation, and decision boundary visualization.

---

## 1. Dataset Description

A synthetic two-dimensional binary classification dataset was generated using `make_classification` with the following parameters:

- 500 samples  
- 2 informative numerical features  
- No redundant features  
- Two balanced classes  
- Random state set for reproducibility  

The dataset allows clear separation between two classes, making it suitable for logistic regression.

---

## 2. Logistic Regression Implementation

The model was implemented without using Scikit-Learn.  
The following components were built manually:

### 2.1 Sigmoid Activation  
The logistic (sigmoid) function was implemented as  
*s(z) = 1 / (1 + exp(-z))*.

### 2.2 Binary Cross-Entropy Loss  
The gradients were derived based on the logistic loss function.

### 2.3 Gradient Descent Optimization  
Weights and bias were updated iteratively across a fixed number of iterations.

### 2.4 Prediction Rule  
Predicted labels were assigned using a decision threshold of 0.5 on the sigmoid output.

---

## 3. Training and Model Parameters

The model was trained using:

- Learning rate: 0.1  
- Iterations: 3000  
- Input: Training split (70% of dataset)

The final learned parameters are printed in the program output:

- Final weights  
- Final bias  

These values vary slightly depending on system environment but remain consistent in structure.

---

## 4. Evaluation Metrics

The following performance metrics were computed on the test split:

- Accuracy  
- Precision  
- Recall  

These provide a quantitative assessment of the classifier’s performance.

---

## 5. Decision Boundary Visualization

A decision boundary plot was generated using a mesh grid evaluated through the trained model.  
The resulting plot was saved as:

```
decision_boundary.png
```

The plot shows:

- The learned separating boundary in the 2D feature space  
- The points colored by their true classes  

This demonstrates how well the model distinguishes between the two classes.

---

## 6. How to Run

Install required packages:

```
pip install numpy scikit-learn matplotlib
```

Run the program:

```
python logistic_regression_from_scratch.py
```

Outputs include:

- Final learned weights and bias  
- Accuracy, precision, and recall  
- Saved image file: `decision_boundary.png`

---

## 7. Deliverable Summary

This submission includes:

- A complete Python implementation of logistic regression from scratch  
- Gradient-based training implementation  
- Evaluation metrics  
- A decision boundary visualization  
- A text-based explanation of methodology and results  

All required tasks and deliverables specified in the project description are fully addressed.
