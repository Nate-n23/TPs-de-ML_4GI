# 🧠 Machine Learning Labs (4GI)

Welcome to the collection of Machine Learning lab sessions. This repository guides you through the full ML lifecycle: from data preparation and regression to clustering and deep learning for medical imaging.

---

## ⚡ Quick Start

**Prerequisites:** You need [Python 3.9+](https://www.python.org/downloads/) and [Git](https://git-scm.com/) installed.

**1. Clone the repository**
```bash
git clone git@github.com:Nate-n23/TPs-de-ML_4GI.git
cd TPs-de-ML_4GI
```

**2. Setup Environment** (Recommended)
```bash
# Verify you have python 3.9+
python3 --version

# Create a virtual environment to keep your system clean
python3 -m venv .venv
source .venv/bin/activate  # On Windows use: .venv\Scripts\activate

# Install all dependencies at once
pip install -r requirements.txt
```

**3. Run the Labs**
Start Jupyter Lab/Notebook to explore the `.ipynb` files:
```bash
jupyter notebook
```
> Then click on `TP1.ipynb` to start the first lab!

---

## 📂 Lab Contents

### [TP1: The User Guide to ML Pipelines](TP1.ipynb)
**Goal:** Predict housing prices using Random Forests.
*   **Concepts:** Data Wrangling, Feature Engineering, geospatial plotting.
*   **Key Tech:** Scikit-learn, Pandas, Joblib.
*   **Outcome:** A serialized Random Forest model ready for deployment.

### [TP2: Advanced Regression & MLOps](TP2.ipynb)
**Goal:** Master regularization and model serving.
*   **Concepts:** Bias-Variance Tradeoff, Ridge vs Lasso (L1/L2), MLflow tracking.
*   **Key Tech:** Docker, MLflow, Flask.
*   **Outcome:** A Dockerized API serving your regression model.

### [TP3: Unsupervised Intelligence](TP3.ipynb)
**Goal:** Discover hidden patterns in dataset.
*   **Concepts:** K-Means, Gaussian Mixture Models (GMM), t-SNE & PCA visualization.
*   **Key Tech:** Scikit-learn, Seaborn.
*   **Outcome:** Comparison of clustering techniques and dimensionality reduction plots.

### [TP4: Medical Computer Vision](TP4.ipynb)
**Goal:** Detect pathologies in Chest X-Rays using Deep Learning.
*   **Concepts:** Convolutional Neural Networks (CNNs), Transfer Learning (ResNet), XAI (Grad-CAM).
*   **Key Tech:** PyTorch, Torchvision, ONNX.
*   **Outcome:** An interpretable Deep Learning model exported for edge deployment.

---

## 🛠 Project Structure

```text
.
├── TP[1-4].ipynb       # The main lab notebooks (Code & Instructions)
├── requirements.txt    # List of all python library dependencies
├── Dockerfile          # For containerizing the TP2 model
├── *.pkl / *.onnx      # Saved trained models (Outputs)
├── *.png / *.pdf       # Visualizations and reports (Outputs)
└── mlruns/             # Directory containing MLflow experiment logs
```

## ❓ FAQ & Troubleshooting

**Q: I get a "ModuleNotFoundError".**
A: Make sure you activated your virtual environment (`source .venv/bin/activate`) and ran `pip install -r requirements.txt`.

**Q: Plots are not showing.**
A: Ensure you run the cell `%matplotlib inline` or `plt.show()` if it's not automatically displaying.

**Q: How do I stop Jupyter?**
A: Press `Ctrl+C` in your terminal.
