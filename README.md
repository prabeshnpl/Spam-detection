# 📧 Spam Detection using Machine Learning

This repository contains an implementation of a **spam message detection** model using Python and scikit-learn. The model classifies SMS messages as either `spam` or `ham` (not spam) using machine learning techniques and natural language processing.

---

## 🔍 Project Overview

The dataset used is a labeled collection of SMS messages categorized as spam or ham. The project covers all standard machine learning pipeline steps:

- Data cleaning & preprocessing
- Text vectorization
- Model training
- Evaluation using classification metrics

---

## 📁 Dataset

The dataset used is `spam.csv` which contains:

| Column    | Description                  |
|-----------|------------------------------|
| Category  | `spam` or `ham` label        |
| Message   | The actual SMS text content  |

- Total messages: 5572
- No missing values

---

## ⚙️ ML Pipeline

- **Preprocessing**:
  - One-hot encoding of labels
  - Text processing with `TfidfVectorizer`
- **Model**:
  - `Support Vector Classifier(SVC)` (best classification algorithm for this datasest)
- **Split**:
  - `train_test_split` used for evaluation

---

## 📈 Results

The model achieves high accuracy on the test set. Key performance metrics include:

- F1-Score
- roc_auc_score
- roc_auc_curve

---

## 🛠 Technologies Used

- Python
- Pandas
- Matplotlib
- Scikit-learn
- TfidfVectorizer
- Jupyter Notebook

---

## ▶️ How to Run

1. Clone the repository
2. Open `spam_detection.ipynb` in Jupyter
3. Run the cells to see the pipeline, model training, and evaluation

```bash
git clone https://github.com/prabeshnpl/Spam-detection.git
cd spam-detection
jupyter notebook spam_detection.ipynb
