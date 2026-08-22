# Fake News Detection System

A Deep Learning based system for detecting whether a given news article is **Fake** or **Real** using Natural Language Processing (NLP) and Deep Learning techniques.

## 📌 Project Overview

The rapid spread of misinformation on digital platforms makes it difficult to distinguish between genuine and misleading news. This project aims to develop an automated Fake News Detection System that analyzes the textual content of a news article and classifies it as either **Fake** or **Real**.

The project uses Natural Language Processing for text preparation and Deep Learning models such as **LSTM** for classification.

## 🎯 Objectives

* Detect fake and real news automatically.
* Perform text preprocessing and NLP-based feature preparation.
* Build a Deep Learning model for news classification.
* Evaluate the model using standard performance metrics.
* Provide a system where users can enter news text and receive a prediction.

## 🛠️ Technologies Used

* **Python**
* **Google Colab**
* **Pandas**
* **NumPy**
* **NLTK**
* **Matplotlib**
* **Seaborn**
* **TensorFlow / Keras**
* **LSTM / BiLSTM**
* **Git & GitHub**

## 📂 Project Structure

```text
fake-news-detection/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   └── Fake_News_Detection.ipynb
│
├── models/
│
├── results/
│
├── README.md
└── requirements.txt
```

### Folder Description

| Folder             | Purpose                        |
| ------------------ | ------------------------------ |
| `data/raw`         | Original dataset files         |
| `data/processed`   | Cleaned and processed data     |
| `notebooks`        | Google Colab/Jupyter notebooks |
| `models`           | Trained Deep Learning models   |
| `results`          | Graphs and evaluation results  |
| `README.md`        | Project documentation          |
| `requirements.txt` | Required Python libraries      |

## 📊 Dataset

The project uses a **Fake and Real News Dataset** containing news articles categorized into two classes:

* `0` → Fake News
* `1` → Real News

After combining and cleaning the dataset, the current dataset contains:

* **44,689 news articles**
* **23,478 Fake News articles**
* **21,211 Real News articles**

The class distribution is approximately:

* Fake News: **52.54%**
* Real News: **47.46%**

The dataset contains the following major fields:

* `title`
* `text`
* `subject`
* `date`

For model training, the **title and article text** are combined into a single `content` field.

## 🔄 Project Workflow

```text
Dataset Collection
       ↓
Data Loading
       ↓
Data Exploration
       ↓
Data Cleaning
       ↓
Text Preprocessing
       ↓
Tokenization
       ↓
Padding
       ↓
Train/Test Split
       ↓
Deep Learning Model
       ↓
Model Training
       ↓
Model Evaluation
       ↓
Fake / Real Prediction
```

## 🔍 Current Progress

### Completed

* [x] Project structure created
* [x] GitHub repository setup
* [x] Google Colab integration
* [x] Dataset collected and extracted
* [x] Dataset loaded and combined
* [x] Fake/Real labels created
* [x] Missing value analysis
* [x] Duplicate analysis
* [x] Exploratory Data Analysis
* [x] Fake vs Real class distribution
* [x] News text length analysis
* [x] Initial data cleaning
* [x] Title and article text combined

### In Progress / Planned

* [ ] Advanced text preprocessing
* [ ] Tokenization
* [ ] Sequence padding
* [ ] Train/Test data splitting
* [ ] LSTM model implementation
* [ ] Model training
* [ ] Model evaluation
* [ ] Confusion matrix
* [ ] Accuracy, Precision, Recall and F1-score
* [ ] BiLSTM/model comparison
* [ ] Fake/Real prediction system
* [ ] Final documentation and presentation

## 🧠 Deep Learning Approach

The primary Deep Learning approach will use an **LSTM (Long Short-Term Memory)** network.

Proposed architecture:

```text
News Text
   ↓
Text Preprocessing
   ↓
Tokenization
   ↓
Padding
   ↓
Embedding Layer
   ↓
LSTM
   ↓
Dropout
   ↓
Dense Layer
   ↓
Sigmoid
   ↓
Fake / Real
```

LSTM is selected because it is designed to process sequential data and can capture important relationships within textual sequences.

## 📈 Model Evaluation

The trained model will be evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Training and Validation Loss
* Training and Validation Accuracy

Different Deep Learning architectures may also be compared to select the best-performing model.

## 🚀 Future Scope

The project can be further improved by:

* Using Bidirectional LSTM or other advanced architectures.
* Applying word embeddings such as Word2Vec or GloVe.
* Using Transformer-based models such as BERT.
* Adding a user-friendly web interface.
* Supporting real-time news analysis.
* Improving robustness against newly emerging misinformation patterns.

## 👥 Team

This project is developed as a **two-member Deep Learning academic project**.

Both members contribute to different stages including dataset preparation, NLP preprocessing, Deep Learning model development, evaluation, documentation, and testing.

## 📚 Academic Project

**Subject:** Deep Learning
**Project:** Fake News Detection System
**Platform:** Google Colab
**Version Control:** GitHub
