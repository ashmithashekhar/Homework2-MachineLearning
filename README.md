Homework 2 — Machine Learning (CS5710)

University of Central Missouri — Fall 2025

Student: Ashmitha Kumbham
Course: CS5710 Machine Learning
Assignment: Home Assignment 2 — Part A (Q1–Q6, theory) & Part B (Q7–Q9, programming)

📂 GitHub Repository: Homework2ML

(All code, PDFs, and explanations are available here.)

Repo Structure

Homework 2 ML(1–6).pdf — Assignment write-up and solutions for Part A (theory).

homework2_7_to_9.py — Python script for Part B (programming).

HOMEWORK2_7_to_9.ipynb — Jupyter/Colab notebook with code + plots.

README.md — this file (full explanations + run instructions).

🔧 How to Run the Code (Part B)
Option 1: Google Colab

Open Google Colab.

Upload homework2_7_to_9.py.

Run all cells (self-contained).

Option 2: Local Python
python -V            # Python 3.9+ recommended
pip install numpy pandas scikit-learn matplotlib
python homework2_7_to_9.py

Part A — Theory (Q1–Q6)
Q1. Decision Stump Prediction

Rule: predict “+” if Sneezing=Yes, else “−”.

Data: (Yes,+), (No,−), (Yes,−), (No,−).

Predictions: +, −, +, − → 1 mistake out of 4.

Training error = 25%.

Memorizer (perfect recall) = 0% error (but poor generalization).

Q2. Training Error as Splitting Criterion

6-row dataset with Age, Exercise, Diet features.

Compute training error for root split:

Age → 16.7%

Exercise → 16.7%

Diet → 16.7%

Best split: tie between all three.

Q3. Entropy & Information Gain

Labels: Yes=3, No=3 → Entropy = 1.0.

After splitting on Exercise: weighted entropy = 0.333.

Information Gain = 0.667 → good split.

Q4. Confusion Matrix Metrics

Confusion matrix (TP=25, FN=5, FP=15, TN=55).

Accuracy = 80%, Precision = 62.5%, Recall = 83.3%, Specificity = 78.6%, F1 ≈ 0.714.

Imbalanced case: accuracy misleads; prefer F1/PR metrics.

Q5. kNN Distance Calculations

Points: A(2,4,Red), B(4,4,Blue), C(4,6,Red); P(5,4).

Distances: d(P,A)=3, d(P,B)=1, d(P,C)=2.24.

1-NN → Blue; 3-NN → Red.

Q6. 4-Fold Cross Validation

Errors:

k=1 → 0.225

k=3 → 0.1625

k=5 → 0.1375

Best generalization: k=5.

Part B — Programming (Q7–Q9)
Q7. Decision Trees on Iris

Train trees with max_depth = 1, 2, 3.

Observations:

Depth=1 → underfit, lower accuracy.

Depth=2/3 → better fit, higher accuracy.

Too deep → risk of overfitting.

Q8. kNN (2 features: sepal length, sepal width)

Train kNN with k=1,3,5,10.

Plots: decision boundaries for each k.

Observations:

k=1 → jagged, high variance.

k=3/5 → smoother, better balance.

k=10 → too smooth, may underfit.

Q9. Performance Evaluation (kNN, k=5)

Compute confusion matrix + classification report.

ROC curves (OvR + micro-average).

Results:

High accuracy (>90%).

ROC/AUC close to 1.0 (well-separated classes).

Micro-AUC shows strong overall separability.

📌 Academic Integrity

Part A: step-by-step derivations based on provided data.

Part B: reproducible Python code with fixed random state.

✍️ Author: Ashmitha Kumbham
📚 Master’s in Data Science and AI, University of central Missouri
