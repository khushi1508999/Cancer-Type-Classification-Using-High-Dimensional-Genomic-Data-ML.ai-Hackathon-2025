# Cancer-Type-Classification-Using-High-Dimensional-Genomic-Data-ML.ai-Hackathon-2025
### ML.ai Hackathon 2025 – Final Project | IITG.ai
A machine learning project for multi-class cancer type classification using high-dimensional RNA-Seq data. Built as part of the ML.ai Hackathon 2025 hosted by IITG.ai, this project tackles imbalanced data, limited labels, and genomic complexity to deliver robust predictive models.

---
## 📌 Problem Statement
The challenge is to classify **five types of cancer** from gene expression profiles using machine learning techniques. The dataset consists of:
- **14,572 gene expression features**
- **Limited labeled data** (only 150 out of 400 training samples)
- **Class imbalance** and **high dimensionality**
  
The project aims to build **robust and generalizable models** that can operate in real-world biomedical contexts like **precision oncology**.

---
## Dataset
Dataset can be accesses through the link mentioned: <https://www.kaggle.com/competitions/ml-ai-hackathon-2025/data>

## 📂 Dataset Overview

| File                  | Description                                                  |
|-----------------------|--------------------------------------------------------------|
| `train.csv`           | 400 samples (150 labeled, 250 unlabeled) × 14,572 gene features |
| `train_labels.csv`    | Labels for 150 samples                                        |
| `test.csv`            | 401 samples (unlabeled)                                       |
| `sample_submission.csv` | Format to follow for final submission                        |

### 🧬 Features
- **Id**: Sample ID (e.g., sample_001)
- **gene_1 to gene_14572**: Real-valued RNA-Seq expression levels
- **Class**: Target cancer type (0–4)

---

## 🎯 Objective

To train a machine learning model that can accurately predict the cancer type (0–4) from gene expression data and **maximize the Macro F1-Score**, which gives equal importance to each class regardless of its frequency.

---

## 🧠 Approach

- ✅ Exploratory Data Analysis (EDA)
- ✅ Dimensionality Reduction (PCA)
- ✅ Feature Selection
- ✅ Semi-Supervised Learning Techniques
- ✅ Model Building using:
  - Random Forest
  - XGBoost
  - LightGBM
- ✅ Hyperparameter Tuning (Grid Search & Stratified K-Fold CV)
- ✅ Final Ensemble Prediction

---

## 📈 Evaluation Metric

The **Macro F1-Score** is used to evaluate model performance.

> It is the unweighted mean of F1 scores calculated per class, ensuring equal importance is given to all five cancer types.

---

## 💡 Key Challenges Tackled

- 🧪 **High-dimensional data** (14,572 features)
- 🔍 **Small labeled dataset**
- ⚖️ **Imbalanced classes**
- 🧠 **Feature engineering** and **robust model selection**
- 💬 **Documented and interpretable pipeline**

---

## 🛠️ Requirements

Install dependencies via:

```bash
pip install -r requirements.txt
