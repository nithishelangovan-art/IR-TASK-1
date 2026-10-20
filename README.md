# Task 1: TF-IDF in Action — Build, Compute, Rank and Explain

##  Project Overview

This project demonstrates **Term Frequency–Inverse Document Frequency (TF-IDF)**, an Information Retrieval technique used to measure the importance of words in a document relative to a collection of documents.

The project uses a cybersecurity document collection to calculate TF, DF, IDF, and TF-IDF scores and retrieve the most relevant documents for given queries using cosine similarity.

##  Objectives

- Create a collection of 10 cybersecurity documents.
- Preprocess text using lowercase conversion, tokenization, stop-word removal, and stemming.
- Calculate Term Frequency (TF).
- Calculate Document Frequency (DF) and Inverse Document Frequency (IDF).
- Construct the TF-IDF matrix.
- Rank documents for search queries using cosine similarity.
- Test a query containing terms absent from the document collection.

## Technologies Used

- Python
- Google Colab / Jupyter Notebook
- Pandas and NumPy
- Scikit-learn
- NLTK
- Matplotlib (if used for visualizations)

##  Dataset

The dataset contains 10 cybersecurity-related documents covering:

1. Phishing Email Attacks
2. Malware and Antivirus Protection
3. Ransomware Incident Response
4. Network Firewalls and Intrusion Detection
5. Encryption and Data Privacy
6. Password Managers and Strong Authentication
7. Cloud Security and Access Control
8. Public Wi-Fi and Safe Browsing
9. Data Breaches and Security Awareness
10. Multi-Factor Authentication

##  Methodology

### 1. Text Preprocessing
Convert text to lowercase, tokenize it, remove stop words, and apply stemming.

### 2. Term Frequency (TF)
Count how frequently each term occurs in each document.

### 3. Document Frequency (DF)
Count the number of documents in which each term appears.

### 4. Inverse Document Frequency (IDF)

The IDF value is calculated using:

\[
IDF(t)=\log_{10}\left(\frac{N}{DF(t)}\right)
\]

Where:
- \(N\) = total number of documents
- \(DF(t)\) = number of documents containing term \(t\)

### 5. TF-IDF Calculation

\[
TFIDF(t,d)=TF(t,d)\times IDF(t)
\]

### 6. Document Ranking

Cosine similarity measures the similarity between a query vector and document vectors. Documents are ranked in descending order of similarity scores.

## 🔎 Sample Search Queries

- `phishing email security`
- `network firewall protection`
- `password encryption privacy`

An additional query, `quantum teleportation`, is used to test terms absent from the collection.

## 📊 Results

The project generates the following result files:

- `document_collection_preprocessed.csv`
- `tf_matrix.csv`
- `df_idf_table.csv`
- `tfidf_matrix.csv`
- `ranked_retrieval_results.csv`

These files show the preprocessed collection, term frequencies, IDF values, TF-IDF weights, and ranked retrieval results.

##  Conclusion

This project demonstrates how TF-IDF represents the importance of terms in documents and how cosine similarity can rank documents according to their relevance to a search query. It provides a basic implementation of a text-based Information Retrieval system using cybersecurity documents.

## Submission

**Course:** Information Retrieval  
**Task:** Task 1 — TF-IDF in Action

