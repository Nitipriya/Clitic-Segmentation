# Clitic Segmentation using Machine Learning

## 📌 Overview

This project focuses on **automatic clitic segmentation** using a machine learning pipeline.
Clitics are linguistic units that attach to words (e.g., prefixes/suffixes), and correctly segmenting them is important for downstream NLP tasks like parsing, translation, and morphological analysis.

The project frames clitic segmentation as a **character-level sequence labeling problem** and uses a **BIO tagging scheme** to identify segmentation boundaries.

---

## 🎯 Objectives

* Build a robust pipeline for clitic segmentation
* Handle orthographic and accent variations effectively
* Compare model performance using evaluation metrics
* Improve segmentation accuracy through feature engineering

---

## 🧠 Approach

### 1. Problem Formulation

* Converted segmentation into a **BIO tagging task**

  * **B** → Beginning of a segment
  * **I** → Inside a segment
  * **O** → Outside / non-boundary

---

### 2. Feature Engineering

* Character-level features
* Contextual **n-grams**
* Position-based features

---

### 3. Model Used

* **Logistic Regression**

  * Chosen for simplicity, interpretability, and strong baseline performance on structured features

---

### 4. Pipeline

1. Data preprocessing
2. Feature extraction
3. Model training
4. Prediction
5. Evaluation

---

### 5. Evaluation Strategy

* Custom **boundary-based F1 score**
* Focuses on:

  * Correct segmentation boundaries
  * Robustness to minor spelling variations

---

## 📊 Results

* Achieved reliable segmentation performance using a lightweight model
* Custom evaluation helped overcome traditional token mismatch issues
* Demonstrated effectiveness of character-level modeling

---

## 📁 Project Structure

```
Clitic-Segmentation/
│
├── data/               # Dataset files
├── notebooks/          # Jupyter notebooks
└── README.md
```

---

## ⚙️ Installation

```bash
git clone https://github.com/Nitipriya/Clitic-Segmentation.git
cd Clitic-Segmentation
pip install -r requirements.txt
```

---

## ▶️ Usage

Run the notebook:

```bash
jupyter notebook notebooks/
```

Or execute the pipeline script:

```bash
python main.py
```

---

## 🔍 Key Learnings

* Character-level modeling is effective for morphological tasks
* Feature engineering plays a crucial role in classical ML approaches
* Custom evaluation metrics can significantly improve insight into model performance

---

## 🚀 Future Improvements

* Use deep learning models (BiLSTM, Transformers)
* Add attention mechanisms for better context understanding
* Expand dataset for better generalization
* Deploy as an API or web tool

---

## 👩‍💻 Author

**Niti Priya**


