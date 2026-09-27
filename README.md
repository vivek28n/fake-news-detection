# Fake News Detection System

A Deep Learning based Fake News Detection System that uses Natural Language
Processing (NLP) techniques to classify news articles as Fake or Real.

## 👥 Team Members

- Vivek Nigam
- Riddhima Tripathi

## 📌 Project Overview

Fake news and misinformation have become major challenges in the digital
world. This project aims to develop a deep learning based system that can
classify news content as Fake or Real.

The system preprocesses the news text, converts it into numerical sequences
using tokenization and padding, and then applies different deep learning
architectures for classification.

## 🎯 Objectives

- Detect whether a given news article is Fake or Real.
- Apply Natural Language Processing techniques to news text.
- Compare different deep learning architectures.
- Evaluate models using standard classification metrics.
- Provide predictions for new user-provided news text.

## 🗂️ Dataset

The project uses the Fake News dataset containing two separate files:

- `Fake.csv` - Fake news articles
- `True.csv` - Real news articles

The two datasets are combined and shuffled before preprocessing.

The dataset contains information such as:

- Title
- News text
- Subject
- Date

A binary label is added:

- `0` → Fake News
- `1` → Real News

## 🔄 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Title + Article Combination
   ↓
Text Preprocessing
   ↓
Tokenization
   ↓
Padding
   ↓
Train-Test Split
   ↓
Deep Learning Models
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Model Comparison
   ↓
New Text Prediction
🧹 Data Preprocessing
The following preprocessing steps are applied:
- Convert text to lowercase
- Remove URLs
- Remove HTML tags
- Remove non-alphabetic characters
- Remove extra spaces
- Remove English stopwords
- Combine news title and article text
The cleaned text is then converted into numerical sequences using a Keras
Tokenizer and padded to a fixed length.
🧠 Deep Learning Models
Three deep learning architectures are implemented.
1. LSTM
Long Short-Term Memory (LSTM) is a recurrent neural network architecture
that can capture sequential patterns in text.
Architecture:
Embedding
    ↓
LSTM
    ↓
Dropout
    ↓
Dense
    ↓
Sigmoid
2. BiLSTM
Bidirectional LSTM processes the sequence in both forward and backward
directions, allowing the model to use information from both directions.
Architecture:
Embedding
    ↓
Bidirectional LSTM
    ↓
Dropout
    ↓
Dense
    ↓
Sigmoid
3. CNN + BiLSTM Hybrid
The hybrid model combines convolutional and bidirectional recurrent layers
to capture local text patterns and sequential information.
Architecture:
Embedding
    ↓
Conv1D
    ↓
Bidirectional LSTM
    ↓
Dropout
    ↓
Dense
    ↓
Sigmoid
📊 Model Evaluation
The models are evaluated using:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
| Model | Accuracy | Precision | Recall | F1 |
|---|---:|---:|---:|---:|
| LSTM | 97.00% | 98.37% | 95.26% | 96.79% |
| BiLSTM | 99.85% | 99.86% | 99.83% | 99.85% |
| CNN + BiLSTM | **99.89%** | **99.93%** | **99.83%** | **99.88%** |
These results are obtained on the held-out test set used in the notebook.
📈 Results
The implemented models were able to classify the test dataset with high
performance.
The project also includes:
- Training and validation accuracy graphs
- Training and validation loss graphs
- Confusion matrices
- Classification reports
- Model performance comparison
🔮 Prediction
The trained hybrid model can be used to classify new text entered by the
user.
Example:
Input News
    ↓
Text Cleaning
    ↓
Tokenization
    ↓
Padding
    ↓
CNN + BiLSTM Model
    ↓
Fake / Real Prediction
🛠️ Technologies Used
- Python
- Google Colab
- Pandas
- NumPy
- NLTK
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- Git
- GitHub
📁 Project Structure
fake-news-detection/
│
├── data/
│   └── raw/
│       ├── Fake.csv
│       └── True.csv
│
├── notebooks/
│   └── Fake_News_Detection.ipynb
│
├── models/
│   ├── fake_news_hybrid_model.keras
│   └── tokenizer.pkl
│
├── README.md
└── requirements.txt
🚀 Future Scope
The project can be further extended by:
- Experimenting with Transformer-based architectures such as BERT.
- Using larger and more diverse datasets.
- Supporting multilingual fake news detection.
- Developing a web-based interface for users.
- Adding real-time news verification features.
- Integrating reliable external sources for fact verification.
- Improving robustness against newly emerging forms of misinformation.
⚠️ Limitations
The model learns patterns from the dataset used for training and testing.
Therefore, its predictions should not be treated as independent factual
verification of a news article.
Performance on new sources, topics, writing styles, or unseen types of
misinformation may differ from the reported test-set results.
📚 Academic Project
This project was developed as part of an academic Deep Learning project.
Team
Vivek Nigam & Riddhima Tripathi

### Ab GitHub mein kya karna hai

Repo mein:

**`README.md` → Edit ✏️ → pura old content replace → above content paste → Commit changes**

Commit message:

```text
Update README with final project details and results
