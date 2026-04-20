pip install spacy
python -m spacy download en_core_web_sm
# 🧠 CS5710 – Machine Learning

## 📌 Home Assignment 4 – NLP Tasks

### 👤 Student Information

* **Name:** *Your Name*
* **Course:** CS5710 Machine Learning
* **University:** University of Central Missouri
* **Semester:** Spring 2026

---

## 📖 Project Overview

This assignment focuses on implementing Natural Language Processing (NLP) tasks using Python. The project demonstrates text preprocessing, linguistic analysis, and entity recognition using modern NLP tools.

---

## ⚙️ Technologies Used

* Python 3.x
* spaCy (NLP library)

---

## 🚀 Installation Instructions

1. Install Python (if not already installed)
2. Install required libraries:

```bash
pip install spacy
python -m spacy download en_core_web_sm
```

---

## 📂 Project Structure

```
├── Q1_text_processing.py
├── Q2_ner_pronoun.py
├── README.md
```

---

## 📝 Part C – Coding Tasks

### 🔹 Q1: Text Processing Pipeline

**Steps performed:**

1. Tokenization – Splitting text into words
2. Stopword Removal – Removing common words
3. Lemmatization – Converting words to base form
4. POS Filtering – Keeping only nouns and verbs

**Input:**

```
John enjoys playing football while Mary loves reading books in the library.
```

**Output:**

```
['enjoy', 'play', 'football', 'love', 'read', 'book', 'library']
```

---

### 🔹 Q2: Named Entity Recognition + Ambiguity Detection

**Steps performed:**

1. Applied Named Entity Recognition (NER)
2. Detected pronoun ambiguity using rule-based check

**Input:**

```
Chris met Alex at Apple headquarters in California. He told him about the new iPhone launch.
```

**Output:**

```
Chris - PERSON  
Alex - PERSON  
Apple - ORG  
California - GPE 

