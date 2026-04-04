# Data-Mining-Algorithms-Collection

This project implements **Data Mining and Machine Learning algorithms** in **Python**, including **Reservoir
Sampling**, **Collaborative Filtering**, **K-Means Clustering**, and **NLP Classification**. It was developed
as part of the **MYE012 - Data Mining** course at the **University of Ioannina**.

---

## TABLE OF CONTENTS
1. [Overview](#overview)  
2. [Features](#features)  
3. [Input Data](#input-data)  
4. [Algorithms Implemented](#algorithms-implemented)  
5. [Implementation Details](#implementation-details)  
6. [Usage](#usage)  
7. [License](#license)  
8. [Contact](#contact)

---

## OVERVIEW

The **Data-Mining-Algorithms-Collection** repository consists of three primary modules based on the course assignments:

### **1. Sampling & Exploration**
A foundational module focusing on streaming data and exploratory analysis of movie datasets.
- Implements **Reservoir Sampling** to select K random items uniformly from an unknown stream N.
- Explores dataset distributions (Zipf plots, cumulative frequencies) and performs statistical hypothesis testing (t-test, chi-test).

### **2. Recommender Systems**
A robust recommendation engine built to predict movie ratings.
- Evaluates **User Average (UA)** and **Item Average (IA)** baselines.
- Implements **Singular Value Decomposition (SVD)** for rank-k approximations.
- Features **User-Based Collaborative Filtering (UCF)** and **Item-Based (ICF)** algorithms.

### **3. Clustering & Classification**
Advanced machine learning applications for grouping and predicting movie features.
- Applies **K-Means** and **Agglomerative Clustering** to user rating behavior.
- Uses **TF-IDF** and **Word2Vec** to extract text features from movie overviews.
- Trains various classifiers (Decision Tree, KNN, Logistic Regression, SVM, MLP) to predict movie genres.

---

## FEATURES

### **Statistical & Data Analysis**
- Hypothesis Testing: Verifies assumptions like "longer movies have higher budgets but lower ratings" or gender-based budget disparities.
- Visual Validation: Generates confidence intervals, scatter plots, heatmaps, and elbow/silhouette plots.

### **Recommender Engines**
- Matrix Factorization: Uses SVD to predict ratings without building dense matrices in memory.
- Graph-Based Similarity: Enhances UCF using **Personalized PageRank (PPR)** to calculate user similarities on a weighted graph.
- Optimization Control: Vectorized implementation utilizing strict array operations to achieve execution times under 5 seconds.

---

## INPUT DATA

### **Movie Metadata & Credits**
- Structure: Includes features like `budget`, `revenue`, `genres`, `release_date`, and `vote_average`.
- Text Data: Movie overviews used for NLP classification.

### **Ratings Datasets**
- Samples: 100,000 ratings from 673 users for 9,066 movies (split into 90% train and 10% test subsets).
- Format: Sparse user-movie interactions formatted as `(user_id, movie_id, rating)`.

---

## ALGORITHMS IMPLEMENTED

### **1. Data Mining & Sampling**
- Reservoir Sampling: Single-pass (K) memory uniform sampling.
- Maximum Likelihood Estimation (MLE): Fitting power-law distributions and Expectation-Maximization (EM) for mixture models.

### **2. Recommender Systems & Graph Algorithms**
- Collaborative Filtering: Calculates cosine similarities to find nearest neighbors (k) for rating predictions.
- Personalized PageRank: Random walk with restarts to evaluate structural node similarity.

### **3. Machine Learning**
- Clustering: K-Means optimization evaluated via Silhouette Coefficient and Sum of Squared Errors.
- NLP Pipelines: Stop-word removal and Word2Vec mean pooling.

---

## IMPLEMENTATION DETAILS

- Language: Pure **Python** (Jupyter Notebooks).
- Libraries: Heavily utilizes `pandas` for data wrangling, `numpy`/`scipy` for sparse matrix algebra, and `scikit-learn`/`gensim` for ML and NLP models.
- Architecture: Strictly avoids explicit `for` loops during user/item traversals in favor of highly optimized, vectorized numpy operations.
- Evaluation Metrics: Validated using **RMSE** (Root Mean Square Error) for recommenders and 5-fold cross-validation (Accuracy, Precision, Recall) for classifiers.

---

## USAGE

### **Run the Analysis Notebooks**
1. Navigate to the project directory.
2. Ensure Python 3 and Jupyter are installed (along with `pandas`, `numpy`, `scikit-learn`, `gensim`, etc.).
3. Open the notebooks: `jupyter notebook`
4. Run the `.ipynb` files sequentially (e.g., `Reservoir_Sampling.ipynb`, `ex2_5203.ipynb`, `ex3_5203.ipynb`).
5. Ensure the Kaggle `movies_metadata.csv`, `credits.csv`, and `ratings_small.csv` datasets are placed in the root directory.

---

## LICENSE

This project was developed for academic purposes as part of the **MYE012 - Data Mining** course at the University of Ioannina.

Final implementation by the project creators.

---

## CONTACT

**Christos-Grigorios Gkovaris** University of Ioannina – Computer Science and Engineering  
GitHub: [ChristosGkovaris](https://github.com/ChristosGkovaris)