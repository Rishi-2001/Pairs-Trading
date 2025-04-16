#Clustering-Based Pairs Trading Strategy
This project explores Pairs Trading by applying unsupervised machine learning clustering algorithms on S&P 500 stock data. The goal is to identify statistically correlated stock pairs using various clustering methods and apply cointegration techniques to build a trading strategy.

📁 Contents
1. Problem Definition

2. Data & Libraries

3. Exploratory Data Analysis (EDA)

4. Data Preparation

5. Clustering Models

6. Pair Selection

7. Conclusion

🔍 Problem Definition
The objective is to perform clustering analysis on S&P 500 stock price data and identify pairs of stocks suitable for a mean-reverting pairs trading strategy.

📦 Data & Libraries
Data Source: Yahoo Finance (via pandas_datareader)

Time Frame: From 2018 onwards

Libraries Used:

pandas, numpy, matplotlib, seaborn

scikit-learn, scipy

pandas_datareader for financial data

statsmodels (likely used later for cointegration, not shown here)

📊 Exploratory Data Analysis (EDA)
View dataset shape and summary statistics

Visualize stock price movements

Understand variance and trends in prices

🔧 Data Preparation
Cleaning missing data

Standardizing the dataset using StandardScaler

Transforming the time series data for clustering models

📈 Clustering Models
Implemented clustering techniques include:

1. K-Means Clustering
Finding optimal clusters using the elbow method

Visualizing clusters using dimensionality reduction (e.g., PCA/t-SNE)

2. Hierarchical Clustering
Creating dendrograms

Using agglomerative clustering with different linkage methods

3. Affinity Propagation
Clusters without specifying the number of clusters

Visualizing pairwise similarities and responsibilities

4. Evaluation Metrics
Adjusted Mutual Information

Cophenetic correlation (for hierarchical)

🔗 Pair Selection
Cointegration Testing: Check statistical correlation for selected pairs

Visualization: Compare price movements of selected pairs

Pair Selection Criteria: Based on cluster membership and cointegration test results

✅ Conclusion
This project successfully:

Applies unsupervised clustering to group similar stocks

Selects cointegrated pairs for statistical arbitrage

Lays the foundation for backtesting a trading strategy

📂 Files
ClusteringForPairsTrading.ipynb: Main Jupyter notebook

SP500Data.csv: Price dataset for S&P 500 stocks (loaded externally)
