# Document Clustering and Search using Fuzzy C-Means

## Overview
This project performs document clustering using **Fuzzy C-Means (FCM)** on text documents.  
The documents are converted into numerical vectors using **TF-IDF vectorization**.

After clustering, a **cosine similarity based search function** is implemented to retrieve relevant documents based on user queries.

---

## Features

- TF-IDF text vectorization
- Document clustering using **Fuzzy C-Means**
- Visualization of cluster distribution
- Identification of **boundary documents**
- Query-based document search using cosine similarity

---

## Project Workflow

1. Load and preprocess dataset  
2. Convert documents to TF-IDF vectors  
3. Apply **Fuzzy C-Means clustering**  
4. Analyze cluster membership distribution  
5. Identify **boundary documents**  
6. Implement cosine similarity search  
7. Retrieve relevant documents for user queries  

---

## Fuzzy C-Means Clustering

Fuzzy C-Means allows documents to belong to **multiple clusters with different membership values**.

Example membership values:

```
Cluster 0 : 0.42
Cluster 1 : 0.38
Cluster 2 : 0.20
```

This indicates that the document is related to multiple clusters.

---

## Boundary Document Analysis

Boundary documents are documents that belong to **multiple clusters with similar membership scores**.

These documents help identify **overlapping topics between clusters**.

---

## Search Function

A cosine similarity based search system is implemented.

Steps:

1. Convert query to TF-IDF vector
2. Compute cosine similarity with document vectors
3. Rank documents based on similarity
4. Return most relevant results

Example queries:

```
search("machine learning")
search("NASA space exploration")
```

---

## Libraries Used

- Python
- NumPy
- Pandas
- Scikit-learn
- Scikit-fuzzy
- Matplotlib

---

## Installation

Install required libraries:

```
pip install numpy pandas scikit-learn scikit-fuzzy matplotlib
```

---

## How to Run

1. Open the Jupyter Notebook
2. Run all cells sequentially
3. Test queries using the search function

Example:

```
search("machine learning")
search("space exploration")
```

---

## Conclusion

This project demonstrates how **Fuzzy C-Means clustering** can be used for document clustering where documents may belong to multiple topics.

The added **cosine similarity search system** allows users to retrieve relevant documents efficiently.
