# Homework 2 — Machine Learning (CS5710)  
**University of Central Missouri — Fall 2025**  
**Course:** CS5710 Machine Learning  
**Student:** Ashmitha Kumbham  

---

## 📘 Assignment Overview  
**Home Assignment 2**  

- **Part A:** Q1–Q6 (theory)  
- **Part B:** Q7–Q9 (programming)  

📂 **Repository:** Homework2ML  
_All code, PDFs, and explanations are included in this repository._  

---

## 📑 Repository Structure  
- **Homework 2 ML(1–6).pdf** → Assignment write-up and solutions for Part A (theory).  
- **homework2_7_to_9.py** → Python script for Part B (programming).  
- **HOMEWORK2_7_to_9.ipynb** → Jupyter/Colab notebook with code + plots.  
- **README.md** → This file (full explanations + run instructions).  

---

## 🔧 How to Run the Code (Part B)  

### Option 1: Google Colab  
1. Open **Google Colab**.  
2. Upload `homework2_7_to_9.py`.  
3. Run all cells (self-contained).  

### Option 2: Local Python Environment  
```bash
# Check Python version
python -V   # Python 3.9+ recommended

# Install required packages
pip install numpy pandas scikit-learn matplotlib

# Run the script
python homework2_7_to_9.py
📘 Part A — Theory (Q1–Q6)
Q1. Decision Stump Prediction
Rule: predict “+” if Sneezing=Yes, else “−”.

Data: (Yes,+), (No,−), (Yes,−), (No,−).

Predictions: +, −, +, − → 1 mistake out of 4 (25% error).

Memorizer (perfect recall) → 0% error (but poor generalization).

Q2. Training Error as Splitting Criterion
Dataset: 6 rows with Age, Exercise, Diet features.

Training errors at root split:

Age → 16.7%

Exercise → 16.7%

Diet → 16.7%

✅ Best split: tie across all three.

Q3. Entropy & Information Gain
Labels: Yes=3, No=3 → Entropy = 1.0

Split on Exercise → weighted entropy = 0.333

Information Gain = 0.667 → good split

Q4. Confusion Matrix Metrics
Confusion matrix: TP=25, FN=5, FP=15, TN=55

Metrics:

Accuracy = 80%

Precision = 62.5%

Recall = 83.3%

Specificity = 78.6%

F1 ≈ 0.714

⚠️ Imbalanced case → Accuracy is misleading; F1/PR are better.

Q5. kNN Distance Calculations
Points: A(2,4,Red), B(4,4,Blue), C(4,6,Red); P(5,4)

Distances:

d(P,A) = 3

d(P,B) = 1

d(P,C) = 2.24

Results:

1-NN → Blue

3-NN → Red

Q6. 4-Fold Cross Validation
Errors:

k=1 → 0.225

k=3 → 0.1625

k=5 → 0.1375

✅ Best generalization: k=5

💻 Part B — Programming (Q7–Q9)
Q7. Decision Trees on Iris Dataset
Trained with max_depth = 1, 2, 3

Observations:

Depth=1 → underfit, low accuracy.

Depth=2/3 → better accuracy, good fit.

Too deep → overfitting risk.

Q8. kNN with (sepal length, sepal width)
Trained with k=1, 3, 5, 10

Observations:

k=1 → jagged decision boundaries (high variance).

k=3/5 → smoother, better trade-off.

k=10 → too smooth, underfit.

Q9. Performance Evaluation (k=5)
Confusion matrix + classification report.

ROC Curves (OvR + micro-average).

Results:

Accuracy > 90%

ROC/AUC ≈ 1.0 → strong separability

Micro-AUC confirms good overall performance.

📌 Academic Integrity
Part A: Step-by-step derivations from provided data.

Part B: Reproducible Python code with fixed random states.

✍️ Author
Ashmitha Kumbham
📚 Master’s in Data Science and AI
University of Central Missouri

