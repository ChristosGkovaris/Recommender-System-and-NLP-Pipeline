# RECOMMENDER SYSTEM AND NLP PIPELINE

This repository contains three **Python-based data mining projects** covering exploratory data analysis, recommender systems, clustering, text classification, and graph-based recommendation methods. The projects were developed as part of the **MYE012 – Data Mining** course at the **University of Ioannina**.

---

## TABLE OF CONTENTS

1. [Overview](#overview)
2. [Tech Stack](#tech-stack)
3. [Features](#features)
4. [Architecture](#architecture)
5. [Project Structure](#project-structure)
6. [Input Data](#input-data)
7. [Algorithms Implemented](#algorithms-implemented)
8. [Installation](#installation)
9. [Usage](#usage)
10. [Contributors](#contributors)
11. [License](#license)
12. [Contact](#contact)

---

## OVERVIEW

The repository consists of three independent coursework projects focused on different areas of data mining and machine learning.

The projects cover:

- Streaming-data sampling with Reservoir Sampling
- Exploratory and statistical analysis of movie metadata
- Rating prediction through baseline and collaborative filtering methods
- Sparse-matrix factorization using Singular Value Decomposition
- Movie clustering based on user-rating behavior
- Text-based movie genre classification
- Personalized PageRank for graph-based user similarity

The implementations combine data processing, statistical analysis, sparse matrix operations, machine learning, natural language processing, and graph algorithms.

---

## TECH STACK

- **Language:** Python
- **Data Processing:** Pandas, NumPy
- **Scientific Computing:** SciPy
- **Machine Learning:** scikit-learn
- **Natural Language Processing:** NLTK, Gensim
- **Graph Processing:** NetworkX
- **Visualization:** Matplotlib, Seaborn
- **Sparse Data Structures:** SciPy sparse matrices
- **Environment:** Google Colab / Jupyter Notebook

---

## FEATURES

- **Sampling & Exploratory Analysis**
  - Reservoir Sampling over streaming input
  - Dataset cleaning and transformation
  - Distribution and Zipf analysis
  - Correlation analysis
  - Statistical hypothesis testing
  - Genre and director analysis

- **Recommender Systems**
  - User Average and Item Average baselines
  - SVD-based rating prediction
  - User-Based Collaborative Filtering
  - Item-Based Collaborative Filtering
  - Centered-rating collaborative filtering
  - RMSE-based model evaluation

- **Clustering & Classification**
  - K-Means clustering
  - Agglomerative clustering
  - Dimensionality reduction with Truncated SVD
  - Cluster interpretation through genre lift
  - TF-IDF and word-embedding text representations
  - Multiple supervised classification models
  - 5-fold stratified cross-validation

- **Graph-Based Recommendation**
  - User similarity graph construction
  - Personalized PageRank
  - PageRank-weighted collaborative filtering

---

## ARCHITECTURE

The repository is organized into three independent coursework modules.

- **Exercise 1** focuses on data sampling and exploratory statistical analysis.
- **Exercise 2** focuses on matrix-based and neighborhood-based recommender systems.
- **Exercise 3** combines unsupervised learning, supervised text classification, and graph-based recommendation.

Each project operates directly on external datasets and implements the corresponding analytical or machine-learning workflow independently.

---

## PROJECT STRUCTURE

```text
.
├── exercise-1-sampling-exploration/
│   ├── reservoir_sampling.py
│   ├── exploration.py
│   └── README.md
│
├── exercise-2-recommender-systems/
│   ├── ex2_5203.py
│   └── README.md
│
├── exercise-3-clustering-classification/
│   ├── ex3_5203.py
│   └── README.md
│
└── README.md
```

---

## INPUT DATA

The projects use movie-related datasets containing:

- Movie metadata
- User ratings
- Movie identifiers
- Movie genres
- Plot overviews
- Credits and crew information
- Train/test rating splits

Depending on the exercise, the source files include:

```text
movies_metadata.csv
credits.csv
ratings_small.csv
links_small.csv
data_train.csv
data_test.csv
input-A.csv
```

---

## ALGORITHMS IMPLEMENTED

### Sampling & Statistical Analysis

- Reservoir Sampling
- Pearson correlation
- Welch's t-test
- Chi-square test of independence
- Zipf and cumulative-frequency analysis

### Recommender Systems

- User Average
- Item Average
- Truncated Singular Value Decomposition
- User-Based Collaborative Filtering
- Mean-centered User-Based Collaborative Filtering
- Item-Based Collaborative Filtering
- Cosine similarity

### Clustering

- K-Means
- Agglomerative Clustering
- Truncated SVD dimensionality reduction
- SSE / elbow analysis
- Silhouette evaluation
- Genre lift and entropy analysis

### Classification

- TF-IDF
- Pre-trained word embeddings with mean pooling
- Decision Tree
- k-Nearest Neighbors
- Logistic Regression
- Support Vector Machine
- Multilayer Perceptron
- Stratified 5-fold cross-validation

### Graph-Based Recommendation

- User similarity graph construction
- Personalized PageRank
- PageRank-weighted User Collaborative Filtering

---

## INSTALLATION

1. Clone the repository:

```bash
git clone <repository-url>
cd <repository-directory>
```

2. Ensure Python and the required libraries are installed:

```bash
pip install pandas numpy scipy scikit-learn matplotlib seaborn nltk gensim networkx
```

3. Place the required datasets in the corresponding exercise directories.

---

## USAGE

Each exercise is executed independently.

For script versions:

```bash
python reservoir_sampling.py
python exploration.py
python ex2_5203.py
python ex3_5203.py
```

The source files were generated from Google Colab notebooks and may also be executed interactively in a compatible notebook environment.

Refer to each exercise README for its required datasets and implemented workflow.

---

## CONTRIBUTORS

- **Christos Gkovaris** — GitHub: [ChristosGkovaris](https://github.com/ChristosGkovaris)

---

## LICENSE

No formal software license is included in the provided project files.

This repository contains academic projects developed as part of the **MYE012 – Data Mining** course at the **University of Ioannina**.

---

## CONTACT

**Christos Gkovaris**  
Computer Science and Engineering  
University of Ioannina  