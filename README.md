# 📈 Hierarchical Clustering on Stock Market Behavior (NSE Stocks)
### Day 13 — 100 Days of AI/ML

This project uses **Hierarchical (Agglomerative) Clustering** to identify behavior-based groups of Indian NSE stocks using 3 years of historical price data.

The goal is to understand which stocks move similarly, share risk levels, or show unique patterns — a common technique in portfolio analysis and quantitative finance.

---

##  Project Objectives
- Download historical *Close* prices using `yfinance`
- Compute daily returns for each stock
- Extract behavior-based features:
  - Annualized mean return  
  - Annualized volatility  
  - Skewness of returns  
  - Maximum drawdown  
  - Average correlation with other stocks  
- Scale the feature data
- Build a **Dendrogram** to visualize hierarchical relationships
- Perform **Agglomerative Clustering (Ward linkage)**
- Visualize clusters using **PCA scatter plot**
- Generate a **correlation heatmap** (cluster-ordered)
- Produce final cluster assignments + summary table

---
##  Dataset
The project uses 10 NSE-listed stocks:
RELIANCE.NS
TCS.NS
INFY.NS
HDFCBANK.NS
ICICIBANK.NS
WIPRO.NS
BAJAJFINSV.NS
HCLTECH.NS
KOTAKBANK.NS
SBIN.NS


Data Period: **2022–2025** (approx. 3 years)

---

##  Techniques Used
- **Hierarchical Clustering (Ward)**  
- **Feature Engineering for Financial Time Series**  
- **Standardization (Z-score scaling)**  
- **PCA for Dimensionality Reduction & 2D Visualization**  
- **Correlation Analysis**  
- **Max Drawdown Computation**

---

## Key Results

### **Cluster Output**
Cluster 0: TCS.NS, BAJAJFINSV.NS, HCLTECH.NS
Cluster 1: RELIANCE.NS, HDFCBANK.NS, ICICIBANK.NS, KOTAKBANK.NS
Cluster 2: SBIN.NS
Cluster 3: INFY.NS, WIPRO.NS


###  Interpretation
- **Cluster 0** → Mixed Tech–Finance group, moderate return & volatility  
- **Cluster 1** → Large-cap stable performers (banking + Reliance)  
- **Cluster 2 (Single)** → SBIN behaves uniquely with higher volatility  
- **Cluster 3** → IT-based twin cluster (Infosys + Wipro)

---

##  Visualizations
- Dendrogram  
- PCA Cluster Plot  
- Cluster-Ordered Correlation Heatmap  

Each plot highlights how stocks relate and why they group together.

---

##  Tools & Libraries
- Python  
- yfinance  
- pandas  
- numpy  
- scipy  
- scikit-learn  
- seaborn  
- matplotlib  

---

##  Conclusion
This mini-project demonstrates how Hierarchical Clustering can uncover **hidden structure in stock market behavior**. Such techniques are used in portfolio optimization, risk grouping, and factor analysis.

This was completed as part of my **Day 13 of 100 Days of AI/ML Challenge**.

---




