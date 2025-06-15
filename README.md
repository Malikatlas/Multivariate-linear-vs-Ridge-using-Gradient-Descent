# Linear vs Ridge Regression - Muscle Mass Prediction

This project compares **Multivariate Linear Regression** and **Ridge Regression** for predicting the **muscle mass percentage** of individuals using:
- Daily Protein Intake (g)
- Exercise Hours per Week
- Hydration Level (liters/day)

Both models are implemented using **Gradient Descent** with the same dataset.

---

### 📌 Problem Statement

Given a health dataset, we:
1. Perform **3 iterations of Gradient Descent** for:
   - Linear Regression (without regularization)
   - Ridge Regression (with L2 regularization α = 0.1)
2. Initialize all parameters (w₁, w₂, w₃, b) to zero
3. After each iteration:
   - Report updated weights and bias
   - Compute Mean Squared Error (MSE)
4. Predict the muscle mass percentage for a new individual with:
   - 105g protein/day
   - 7.5 hours exercise/week
   - 3.6L hydration/day
5. Discuss:
   - The impact of learning rate
   - Differences between L1 and L2 regularization
   - How regularization prevents overfitting

---

### 📊 Dataset

| Protein (g) | Exercise (hrs/wk) | Hydration (L/day) | Muscle Mass (%) |
|-------------|-------------------|-------------------|------------------|
| 80          | 5                 | 3.0               | 45               |
| 100         | 7                 | 3.5               | 50               |
| 90          | 6                 | 3.2               | 48               |
| 110         | 8                 | 4.0               | 55               |
| 95          | 6.5               | 3.8               | 50               |

---

### ⚙️ Model Settings

| Model               | α (Regularization) | η (Learning Rate) | Iterations |
|--------------------|--------------------|--------------------|------------|
| Linear Regression   | 0                  | 0.0001             | 3          |
| Ridge Regression    | 0.1                | 0.0001             | 3          |

---

### 🧠 Key Concepts

- **Gradient Descent**: Iteratively optimizes weights by minimizing the loss.
- **Ridge Regression (L2)**: Adds penalty on weights to control overfitting.
- **L1 vs L2**:
  - **L1** (Lasso): Can reduce some weights to exactly zero (feature selection).
  - **L2** (Ridge): Shrinks weights smoothly but doesn’t zero them out.

---

### 🗂️ Files

- `Question.pdf` – Contains the assignment description.
- `Solution.pdf` – Includes handwritten calculations and results for both parts.

---

### 🚀 How to Run (If using Python)
```bash
pip install numpy
python linear_vs_ridge.py
