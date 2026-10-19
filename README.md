# Logistic Regression Classifier Workshop

Binary classification (student pass/fail from hours studied) with logistic regression, binary cross-entropy, and gradient descent.

Jasper Lim
9117038

## Setup

Requires Python 3.10+ and Git.

```powershell
git clone https://github.com/JasperCLim/LogisticRegressionClassifier_Workshop.git
cd LogisticRegressionClassifier_Workshop

python -m venv .venv
.\.venv\Scripts\Activate.ps1        # macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt
```

## How to Run

1. Open the folder in VS Code (with the Jupyter extension) or run `jupyter lab`.
2. Select the `.venv` interpreter as the notebook kernel.
3. Open a notebook and choose **Run All**:
   - [`LogisticRegressionClassifier_Workshop.ipynb`](LogisticRegressionClassifier_Workshop.ipynb): the workshop (sigmoid, scikit-learn model, log-loss, in-class activity).
   - [`PairProgrammingReport.ipynb`](PairProgrammingReport.ipynb): the pair programming deliverable.

## PairProgrammingReport Overview

[`PairProgrammingReport.ipynb`](PairProgrammingReport.ipynb) implements logistic regression from scratch with NumPy:

- **Derivation:** binary cross-entropy loss, its gradient `(1/N) Xᵀ(ŷ − y)`, and the gradient descent update.
- **Code:** vectorized sigmoid, loss, gradient, training loop, and prediction, with a numerical gradient check, loss curve, and decision-boundary plot.
- **Validation:** the learned weights and loss match scikit-learn's unregularized `LogisticRegression`.
- **Talking points:** three points on the implementation, plus three review points on the peer's implementation ([AlamirConestoga/LogisticRegressionClassifier_Workshop](https://github.com/AlamirConestoga/LogisticRegressionClassifier_Workshop)).
