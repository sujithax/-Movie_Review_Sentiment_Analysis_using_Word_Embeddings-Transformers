# Movie Review Sentiment Analysis using Word Embeddings & Transformers
A sentiment analysis project that uses Word2Vec and Sentence Transformer embeddings to represent movie reviews. Random Forest and Neural Network models are used to classify reviews and compare their performance.  Technologies: Python, Pandas, NumPy, Scikit-learn, TensorFlow, Sentence Transformers

##  Project Overview

This project focuses on automatically classifying movie reviews as **Positive** or **Negative** using Natural Language Processing (NLP) and Machine Learning techniques.

Different text representation approaches are explored, including **Word2Vec** and **Sentence Transformer embeddings**, followed by classification using **Random Forest** and a **Neural Network**. The project demonstrates how different embedding techniques can be used to convert text into numerical representations for sentiment prediction.

---

##  Problem Statement

Manually analyzing a large number of movie reviews is time-consuming. This project aims to build an AI-based sentiment analyzer that can automatically understand movie reviews and classify the expressed sentiment as positive or negative.

---

##  Dataset

The dataset contains movie reviews with two columns:

| Column      | Description                                     |
| ----------- | ----------------------------------------------- |
| `review`    | Textual movie review                            |
| `sentiment` | Sentiment label: `0 = Negative`, `1 = Positive` |

The dataset contains **9,982 reviews** after data preparation. There are no missing values in the dataset.

---

##  Project Workflow

```text
Movie Reviews
      ↓
Data Loading & Exploration
      ↓
Data Cleaning
      ↓
Text Preprocessing
      ↓
Text Embeddings
   ↙          ↘
Word2Vec   Sentence Transformer
   ↓              ↓
Random Forest   Neural Network
   ↘              ↙
    Model Evaluation
```

---

##  Data Preparation

The dataset was explored and prepared before model training.

The following steps were performed:

* Loaded the dataset using Pandas
* Checked the dataset shape
* Checked for missing values
* Checked for duplicate records
* Removed duplicate records
* Reset the DataFrame index
* Examined sentiment distribution

The original dataset contains the `review` and `sentiment` columns, with sentiment represented using binary labels.

---

##  Embedding Techniques

### 1. Word2Vec

Word2Vec is used to convert individual words into numerical vectors that capture relationships between words.

These word embeddings are then used as features for the sentiment classification model.

**Library:** Gensim

### 2. Sentence Transformers

Sentence Transformers are used to generate numerical representations of complete sentences or reviews.

Unlike Word2Vec, which represents individual words, sentence embeddings capture the semantic meaning of the complete text.

**Library:** Sentence Transformers

---

##  Machine Learning Models

### Random Forest

A Random Forest classifier is trained using the generated text embeddings to classify movie reviews into positive and negative sentiment categories.

### Neural Network

A neural network is also built using TensorFlow/Keras to perform sentiment classification using the generated embeddings.

The notebook evaluates model performance using training and testing accuracy.

---

##  Model Evaluation

The models are evaluated using:

* Training Accuracy
* Testing Accuracy
* Confusion Matrix

The project compares the performance of different combinations of:

* Word2Vec + Random Forest
* Word2Vec + Neural Network
* Transformer-based embeddings + classification model

This comparison helps understand how different text representation techniques affect sentiment classification.

---

##  Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Gensim**
* **Scikit-learn**
* **TensorFlow / Keras**
* **Sentence Transformers**
* **PyTorch**
* **Matplotlib**
* **Seaborn**

The notebook imports these libraries for data manipulation, visualization, embeddings, model building, and evaluation.


##  Key Learning Outcomes

Through this project, I explored:

* Natural Language Processing fundamentals
* Text preprocessing and sentiment classification
* Word embeddings using Word2Vec
* Sentence-level embeddings using Transformers
* Random Forest classification
* Neural Network-based classification
* Model evaluation and comparison
* Understanding the difference between traditional word embeddings and transformer-based embeddings

---
