# 📧 Email Spam Detection with LSTM Neural Network

## 🎯 Project Overview

This project implements a deep learning-based email spam detection system using an LSTM (Long Short-Term Memory) neural network. The model achieves **96.2% accuracy** in distinguishing between spam and legitimate (ham) emails through advanced text preprocessing and sequence modeling.

## 🏆 Key Achievements

- **Test Accuracy**: 96.17%
- **Validation Accuracy**: 95.83%
- **Model Type**: LSTM Neural Network
- **Dataset**: Balanced (equal spam/ham distribution)

## 📊 Dataset

The dataset contains **5,171** emails with the following structure:

| Column | Description |
|--------|-------------|
| Unnamed: 0 | Index column |
| label | Email classification (ham/spam) |
| text | Email content |
| label_num | Numeric label (0/1) |

### Data Balance
- Original dataset: Imbalanced (more ham than spam)
- **After balancing**: Equal distribution (approximately 50% spam, 50% ham)

## 🧠 Methodology

### 1. Data Preprocessing

#### Text Cleaning
- Removed 'Subject' prefix from emails
- Removed punctuation using string translation
- Converted text to lowercase
- Removed stopwords (common English words like 'the', 'is', 'at')

#### Word Cloud Visualization
```python
# Word clouds generated for both spam and ham emails
- Spam emails: Keywords like "free", "offer", "cheap", "photoshop"
- Ham emails: Keywords like "meeting", "conference", "project"
