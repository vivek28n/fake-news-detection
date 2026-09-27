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
