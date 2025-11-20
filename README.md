---

# **Transformer-based Patient Record Summarizer**

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-EE4C2C)
![Transformers](https://img.shields.io/badge/Transformers-T5-green)
![License](https://img.shields.io/badge/License-Academic-blueviolet)
![Status](https://img.shields.io/badge/Status-Active-success)

A complete pipeline for **fine-tuning T5 transformers on synthetic clinical records**, evaluating summarization quality with **ROUGE, BLEU, and METEOR**, and visualizing metrics using **matplotlib**.
Designed for **Google Colab / Jupyter Notebook** with auto-installation of dependencies.

---

## 🚀 **Features**

### **✔ Automatic Setup**

Installs missing packages such as `transformers`, `torch`, `rouge_score`, `nltk`, etc.

### **✔ Synthetic Clinical Dataset Generator**

Creates realistic patient records with:

* Disease conditions
* Treatments
* Test findings
* Follow-up duration
* Auto-generated reference summaries

### **✔ Transformer Fine-Tuning**

* Uses **T5-small**
* Custom PyTorch Dataset
* 3-epoch training loop
* AdamW optimizer
* Linear warm-up scheduler

### **✔ Evaluation Metrics**

Computes per-sample and average:

* **ROUGE-1**
* **ROUGE-2**
* **ROUGE-L**
* **BLEU**
* **METEOR**

### **✔ Visualizations**

Generates metric plots:

* ROUGE-1
* ROUGE-L
* BLEU
* METEOR
* Average metric summary

### **✔ Exports Results**

Saves detailed predictions + scores to:

```
/mnt/data/eval_results.csv
```

---

## 📁 **Project Structure**

```
Transformer-based-patient-record-summarizer/
│
├── main_notebook.py / .ipynb     # Full model training + evaluation
├── README.md                     # Documentation (this file)
└── eval_results.csv (generated)  # Saved metrics and predictions
```

---

## 🔧 **Requirements**

The script automatically installs everything, but base dependencies are:

* Python 3.8+
* PyTorch
* Transformers
* NLTK
* rouge_score
* matplotlib
* pandas
* scikit-learn

---

## ▶️ **How to Run**

1. Open the notebook in **Google Colab** or **local Jupyter**
2. Run all cells — the script will:

   * Install packages
   * Create dataset
   * Train the model
   * Evaluate summaries
   * Generate plots
   * Export CSV results

---

## 📊 **Example Output**

### **Sample Generated Summary**

```
Asthma managed with nebulization; follow-up in 5 days.
```

### **Average Evaluation Metrics**

Displayed as:

* ROUGE-1
* ROUGE-2
* ROUGE-L
* BLEU
* METEOR

### **Saved File**

```
/mnt/data/eval_results.csv
```

---

## 🎯 **Applications**

* Clinical text summarization research
* NLP experimentation using transformers
* Academic projects
* Healthcare AI prototyping
* Evaluation benchmarking studies

---

## 📝 **License**

This project is free for **academic and research** use.

---
