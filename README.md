<div align="center">

# 🦁 Support Vector Machine (SVM) — Interactive Masterclass & Visualizer
### **Lindenwood University — Interactive Data Science & Machine Learning Masterclass**

[![Live Interactive Lab](https://img.shields.io/badge/Launch_Interactive_Lab-Live_Demo-C5B358?style=for-the-badge&logo=googlechrome&logoColor=black)](https://sagarkalauni.github.io/support-vector-machine/)
[![Course](https://img.shields.io/badge/Course-DSCI_35600-000000?style=for-the-badge&logo=academia&logoColor=C5B358)](#)
[![Author](https://img.shields.io/badge/Faculty-Sagar_Kalauni,_M.S.-1E293B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SagarKalauni)

</div>

---

## 📖 Overview

An interactive mathematical and visual simulation of **Linear Support Vector Machines (SVM)**. Built for Lindenwood University's Machine Learning course to illustrate maximum-margin separation, support vector identification, slack variables ($\xi_i$), and the trade-off controlled by the regularization parameter $C$.

> 🔗 **Launch the Live Interactive Application:** [**https://sagarkalauni.github.io/support-vector-machine/**](https://sagarkalauni.github.io/support-vector-machine/)

---

### 📐 Mathematical Formulation

Given binary labeled training data ${(\mathbf{x}_i, y_i)}_{i=1}^n$ with $y_i \in \{-1, +1\}$, the **Soft-Margin Primal Optimization Problem** seeks hyperplane $\mathbf{w}^\top \mathbf{x} + b = 0$ that maximizes geometric margin $\frac{2}{\|\mathbf{w}\|_2}$ while allowing margin violations $\xi_i \ge 0$:

$$\underset{\mathbf{w}, b, \boldsymbol{\xi}}{\min} \quad \frac{1}{2} \|\mathbf{w}\|_2^2 + C \sum_{i=1}^{n} \xi_i$$
$$\text{subject to} \quad y_i \left(\mathbf{w}^\top \mathbf{x}_i + b\right) \ge 1 - \xi_i, \quad \xi_i \ge 0 \quad \forall i \in \{1, \dots, n\}$$

Equivalent **Hinge Loss** unconstrained formulation:
$$\mathcal{L}(\mathbf{w}, b) = \frac{1}{2} \|\mathbf{w}\|_2^2 + C \sum_{i=1}^{n} \max\left(0, \, 1 - y_i(\mathbf{w}^\top \mathbf{x}_i + b)\right)$$

---

## ✨ Key Interactive Features

- **Maximum-Margin Street Visualization:** Live rendering of the decision boundary $\mathbf{w}^\top \mathbf{x} + b = 0$ and margin hyperplanes $\mathbf{w}^\top \mathbf{x} + b = \pm 1$.
- **Active Support Vector Highlighting:** Automatically identifies points lying on or inside the margin ($\alpha_i > 0$).
- **Soft-Margin Penalty ($C$) Tuning:** Explore how small $C$ prioritizes a wider street (higher bias, lower variance) vs. large $C$ penalizing slack violations (hard margin limit).
- **Interactive Point Manipulation:** Add or drag outliers to see how only support vectors dictate hyperplane orientation.

---

## 🎓 Pedagogical & Course Context

- **Institution:** Lindenwood University (*College of Science, Technology, and Health*)
- **Course Curriculum:** DSCI 35600 — Machine Learning
- **Instructor & Author:** **Sagar Kalauni, M.S.** (*Full-Time Faculty in Data Science*)
- **Tech Stack:** HTML5, Tailwind CSS, **D3.js** (Dynamic Data Visualization), **MathJax** (LaTeX Mathematical Rendering), Vanilla ES6+ JavaScript (Zero-Dependency Client-Side Execution).

---

## 🚀 Running Locally

Because this visualizer is engineered as a self-contained, zero-build client-side application, you can run it immediately in any modern browser:

```bash
# Clone the repository
git clone https://github.com/SagarKalauni/support-vector-machine.git

# Navigate into the project directory
cd support-vector-machine

# Open index.html directly in your browser or serve locally:
python -m http.server 8000
```

---

## 🔗 Explore the Complete Interactive Masterclass Suite

| Module | Topic | Live Link |
| :--- | :--- | :---: |
| **Linear Regression** | Ordinary Least Squares & Residual Minimization | [Launch](https://sagarkalauni.github.io/linear-regression/) |
| **Logistic Regression** | Sigmoid Probabilities & Binary Cross-Entropy | [Launch](https://sagarkalauni.github.io/logistic-regression/) |
| **Regularization ($L_1 / L_2$)** | Lasso vs. Ridge Constraint Geometry | [Launch](https://sagarkalauni.github.io/Regularization/) |
| **K-Nearest Neighbors** | Instance-Based Learning & Distance Metrics | [Launch](https://sagarkalauni.github.io/knn/) |
| **Support Vector Machine** | Maximum-Margin Hyperplanes & Soft Margin $C$ | [Launch](https://sagarkalauni.github.io/support-vector-machine/) |
| **RBF Kernel SVM** | Non-Linear Kernel Trick & $(\gamma, C)$ Tuning | [Launch](https://sagarkalauni.github.io/rbf-kernel-svm/) |
| **Decision Tree (CART)** | Recursive Splitting, Gini & Entropy | [Launch](https://sagarkalauni.github.io/decision-tree/) |
| **Random Forest** | Bagging & Ensemble Variance Reduction | [Launch](https://sagarkalauni.github.io/random-forest/) |
| **Voting Classifier** | Hard Majority vs. Soft Probability Voting | [Launch](https://sagarkalauni.github.io/voting-classifier/) |
| **K-Means Clustering** | Lloyd's Algorithm, Voronoi & Elbow WCSS | [Launch](https://sagarkalauni.github.io/k-mean-clustering/) |
| **Confusion Matrix** | Precision, Recall, Specificity & $F_1$-Score | [Launch](https://sagarkalauni.github.io/confusion-matrix/) |
| **Confidence vs. Prediction Intervals** | Mean Response vs. Individual Uncertainty | [Launch](https://sagarkalauni.github.io/confidence-and-prediction-interval/) |
| **Bootstrapping** | Non-Parametric Resampling with Replacement | [Launch](https://sagarkalauni.github.io/bootstrap/) |
| **Q-Q Plot** | Gaussian Normality & Tail Diagnostics | [Launch](https://sagarkalauni.github.io/qq-plot/) |
| **Train-Test Split & CV** | Holdout Partitioning & $K$-Fold Cross-Validation | [Launch](https://sagarkalauni.github.io/split/) |
| **One-Hot Encoding** | Categorical Expansion & Dummy Variable Trap | [Launch](https://sagarkalauni.github.io/one-hot-encoding/) |

---

<div align="center">
  <sub>Developed with ❤️ for Data Science students by <a href="https://github.com/SagarKalauni">Sagar Kalauni</a> · <a href="https://sagarkalauni.github.io">Portfolio</a></sub>
</div>
