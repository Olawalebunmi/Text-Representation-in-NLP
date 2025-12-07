# Text-Representation-in-NLP
Text Representation in NLP – Implementations of One-Hot Encoding, Bag of Words, TF‑IDF, Word2Vec, and Gensim word embeddings.

## Text Encoding Methods
Encoding text into numerical form is essential for Natural Language Processing (NLP) models. This document explains several popular approaches to text representation.

1. One‑Hot Encoding
- Represents each word as a binary vector with a single “1” at the index of the word.
- Simple but inefficient for large vocabularies (results in sparse vectors).
- Example:
["cat", "dog", "fish"]
cat → [1,0,0], dog → [0,1,0], fish → [0,0,1]

2. Bag of Words (BoW)
- Counts word occurrences in a document.
- Ignores grammar and order, focusing only on frequency.
- Produces sparse, high‑dimensional vectors.
3. TF‑IDF (Term Frequency – Inverse Document Frequency)
- Extends BoW by weighting words based on importance.
- Common words get lower weights, rare but meaningful words get higher weights.
- Useful for text classification and information retrieval

4. Word2Vec
- Neural network model that learns dense vector representations of words.
- Captures semantic relationships (e.g., king – man + woman ≈ queen).
- Two main architectures: CBOW (predict word from context) and Skip‑Gram (predict context from word).
5. Gensim Word Embeddings
- Python library for training and loading word embeddings.
- Provides pre‑trained models and efficient implementations of Word2Vec, FastText, and more.

## Why Encoding Matters
Encoding transforms text into numerical vectors that machine learning models can process. Choosing the right method depends on the task:
- One‑Hot / BoW → Simple tasks, small datasets
- TF‑IDF → Text classification, document similarity
- Word2Vec / Gensim → Semantic understanding, deep learning models
