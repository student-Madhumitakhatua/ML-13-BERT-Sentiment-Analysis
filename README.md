# ML-13: BERT Sentiment Analysis

## 📌 Project Overview

This project implements sentiment analysis on IMDb movie reviews using a fine-tuned DistilBERT Transformer model.

The system classifies movie reviews into two categories:

* Positive
* Negative

A traditional Machine Learning model is also implemented to compare its performance with DistilBERT.

## 🎯 Objectives

* Perform sentiment classification on movie reviews.
* Fine-tune a pre-trained DistilBERT model.
* Apply text tokenization, padding and truncation.
* Track training and validation loss.
* Evaluate performance using Accuracy and F1-score.
* Compare Transformer-based learning with traditional Machine Learning.
* Save and reload the trained model for prediction.

## 📂 Dataset

**Dataset:** IMDb Movie Reviews
**Source:** Hugging Face Datasets
**Repository:** `stanfordnlp/imdb`

| Label | Sentiment |
| ----- | --------- |
| 0     | Negative  |
| 1     | Positive  |

### Dataset Split

| Dataset    |    Samples |
| ---------- | ---------: |
| Training   |      5,000 |
| Validation |      1,000 |
| Testing    |      5,000 |
| **Total**  | **11,000** |

## 🛠️ Technologies Used

* Python
* PyTorch
* Hugging Face Transformers
* Hugging Face Datasets
* DistilBERT
* Scikit-learn
* Pandas
* NumPy
* Matplotlib

## 🧠 Models Implemented

### 1. DistilBERT

Pre-trained DistilBERT is fine-tuned for binary sentiment classification.

Model: `distilbert-base-uncased`

### 2. TF-IDF + Logistic Regression

A traditional Machine Learning model is implemented as a baseline for performance comparison.

* TF-IDF Vectorization
* Unigrams and Bigrams
* Logistic Regression

## ⚙️ Project Workflow

1. Import required libraries.
2. Load the IMDb dataset.
3. Perform train, validation and test splitting.
4. Load the DistilBERT tokenizer.
5. Tokenize movie reviews.
6. Load the pre-trained DistilBERT model.
7. Prepare training configuration.
8. Fine-tune the model.
9. Track training and validation loss.
10. Evaluate model performance.
11. Implement TF-IDF + Logistic Regression.
12. Compare both models.
13. Save and reload the fine-tuned model.
14. Predict sentiment on five new reviews.

## 📊 Evaluation Metrics

* Accuracy
* F1-score
* Training Loss
* Validation Loss
* Confusion Matrix
* Classification Report

## 💾 Model Saving and Inference

The fine-tuned DistilBERT model and tokenizer are saved in:

`distilbert-imdb-sentiment`

The saved model is reloaded and used to predict the sentiment of five new movie reviews.

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Open the Notebook

Open `ML-13-BERT-Sentiment-Analysis.ipynb`.

### 4. Run the Notebook

Execute all cells sequentially.

**Recommended Environment:** Google Colab with GPU acceleration (T4), if available.

## 📁 Project Structure

```text
ML-13-BERT-Sentiment-Analysis/
│
├── ML-13-BERT-Sentiment-Analysis.ipynb
├── README.md
└── requirements.txt
```

## 👩‍💻 Author

**Madhumita Khatua**

BCA Student | Machine Learning Enthusiast

GitHub: [student-Madhumitakhatua](https://github.com/student-Madhumitakhatua)

---

⭐ This project demonstrates the practical application of Transformer-based Natural Language Processing for movie review sentiment classification.
