# Clustering-Based Pairs Trading Strategy

This project explores **Pairs Trading** using **unsupervised machine learning clustering algorithms** applied to S&P 500 stock data. The goal is to identify statistically correlated stock pairs suitable for mean-reversion strategies.

---

## Problem Statement

We aim to discover stock pairs for a pairs trading strategy using clustering methods such as:

- K-Means Clustering
- Hierarchical (Agglomerative) Clustering
- Affinity Propagation

Once the pairs are formed, **cointegration tests** are used to verify if the stocks are suitable for trading.

---

## Workflow

### 1. Data Loading
- Load S&P 500 historical prices (2018 onward) from Yahoo Finance

### 2. Data Preparation
- Clean missing values
- Normalize the price data using `StandardScaler`

### 3. Clustering Techniques
- **K-Means**:
  - Determine optimal clusters using the elbow method
  - Visualize clusters
- **Hierarchical Clustering**:
  - Generate dendrogram
  - Cluster stocks based on linkage distance
- **Affinity Propagation**:
  - Automatically detects the number of clusters

### 4. Cointegration & Pair Selection
- Select pairs within the same cluster
- Test for cointegration
- Visualize price spreads of selected pairs

---

## Key Takeaways

- Clustering helps in reducing the universe of stocks to a manageable set of similar candidates.
- Cointegration testing improves the statistical validity of selected trading pairs.
- The approach lays the foundation for implementing a complete pairs trading strategy, including backtesting and execution.

---

## Future Work

- Add statistical backtesting of trading signals
- Implement strategy execution and performance metrics
- Integrate DBSCAN and other clustering models

---
