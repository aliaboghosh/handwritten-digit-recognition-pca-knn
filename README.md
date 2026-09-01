# Handwritten Digit Recognition using PCA and KNN

A machine learning project for recognizing handwritten digits using dimensionality reduction and instance-based classification.

The project uses the **scikit-learn Digits dataset**, applies **Principal Component Analysis (PCA)** for dimensionality reduction, and trains a **K-Nearest Neighbors (KNN)** classifier for multi-class digit recognition.

## Project Overview

The dataset contains 1,797 grayscale images representing handwritten digits from 0 to 9.

Each image has a resolution of 8×8 pixels and is flattened into 64 numerical features.

The machine learning pipeline includes:

* Train/Test Split
* Feature Standardization
* Principal Component Analysis (PCA)
* KNN Hyperparameter Selection using Cross-Validation
* Multi-class Classification
* Model Evaluation

## Dimensionality Reduction

PCA was used to reduce the original 64 features while preserving 95% of the dataset variance.

* Original features: 64
* PCA components: 40
* Retained variance: 95%

## Model Selection

Several values of K were evaluated using 5-fold Cross-Validation.

The best-performing configuration was:

`K = 5`

## Results

| Metric            |  Score |
| ----------------- | -----: |
| Accuracy          | 97.22% |
| Precision (Macro) | 97.31% |
| Recall (Macro)    | 97.21% |
| F1-Score (Macro)  | 97.20% |

## Technologies

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## Machine Learning Techniques

* Data Preprocessing
* Standardization
* Principal Component Analysis (PCA)
* K-Nearest Neighbors (KNN)
* Cross-Validation
* Multi-class Classification
* Confusion Matrix Analysis

## Repository Structure

```text
.
├── README.md
├── handwritten_digit_recognition.ipynb
├── requirements.txt
└── figures/
```

## How to Run

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Then open:

```text
handwritten_digit_recognition.ipynb
```

using Jupyter Notebook or JupyterLab.

## Author

Ali Aboghosh
Data Science & Artificial Intelligence Student
