# 📊 Coreset Selection & Anomaly Detection (Linear Algebra Lab 03)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Linear Algebra](https://img.shields.io/badge/Applied-Linear%20Algebra-green.svg)
![Status](https://img.shields.io/badge/Status-Academic%20Project-brightgreen.svg)

---

## 🧠 Overview

This project is an academic lab assignment for the Applied Linear Algebra course.
It demonstrates how linear algebra concepts can be applied to an industrial anomaly detection problem.

Main topics:
- SVD (Singular Value Decomposition)
- Projection matrices (Hat Matrix)
- Leverage scores
- Coreset selection
- Efficient anomaly detection

---

## 🎯 Problem Statement

Industrial inspection systems require processing large datasets of images.
However, using full datasets is computationally expensive.

This project addresses:

> How can we reduce dataset size while preserving geometric structure and detection quality?

---

## ⚙️ Key Idea

Instead of using all data points:

- Compute importance scores (leverage scores)
- Select a representative subset (coreset)
- Perform anomaly detection on reduced data

This reduces computation while maintaining performance.

---

## 🧮 Mathematical Background

### Least Squares
x* = (A^T A)^(-1) A^T b

### Hat Matrix
H = A (A^T A)^(-1) A^T

### Leverage Scores
ℓ_i = H_ii

Using SVD:
A = U Σ V^T
ℓ_i = ||U_i,:||^2

---

## 🧪 Methodology

1. Image patch extraction
2. Feature vector construction
3. Memory bank creation
4. SVD decomposition
5. Leverage score computation
6. Coreset sampling
7. Anomaly detection

---

## 📊 Pipeline

Raw Images
 → Patch Extraction
 → Feature Vectors
 → Matrix A
 → SVD
 → Leverage Scores
 → Coreset Selection
 → Anomaly Detection

---

## 📁 Dataset

MVTec Anomaly Detection (Bottle category)
https://www.kaggle.com/datasets/thtuan/mvtecad-mvtec-ad

---

## 🚀 Results

- Significant dataset reduction
- Faster computation
- Preserved anomaly detection performance

---

## 🛠 Requirements

pip install numpy matplotlib scikit-learn jupyter

---

## ▶️ Run

jupyter notebook Lab#03.ipynb

---

## 👨‍🎓 Academic Info

Course: Applied Linear Algebra
University: Ferdowsi University of Mashhad
Type: Laboratory Project

---

## 👤 Author :‌ Ehsan Soveizi

Academic implementation of:
- Linear algebra theory
- Matrix factorization
- Machine learning application

---

## 📌 Future Work

- GPU-accelerated SVD
- Deep feature extraction
- Real-time anomaly detection
