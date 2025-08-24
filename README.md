# Fashion-MNIST Clustering Analysis

[![Python](https://img.shields.io/badge/Python-3.8+-blue)](https://www.python.org/) 
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.2+-orange)](https://scikit-learn.org/stable/) 
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

---

## Overview
This project performs **unsupervised clustering** on the **Fashion-MNIST dataset** using **K-Means** and **Agglomerative Clustering**.  
Fashion-MNIST contains **70,000 grayscale images** of size 28×28 pixels across **10 categories** (T-shirts, trousers, dresses, etc.).  

The main goals are to:
- Explore how clustering algorithms group images without labels.
- Visualize cluster centroids and sample images.
- Evaluate clustering performance using quantitative metrics.

---

## Key Features

### **1. K-Means Clustering**
- Divides the dataset into **10 clusters**.  
- Uses **k-means++ initialization** for faster and more accurate convergence.  
- **Visualizes cluster centroids** as average images.  
- **Displays sample images** from each cluster with their true labels.

### **2. Agglomerative Clustering**
- Hierarchical clustering on a subset of **500 samples**.  
- Uses **Ward linkage** and **Euclidean distance**.  
- **Visualizes sample images** per cluster.

---

## Data Preprocessing
- Standardizes pixel values with **StandardScaler**.  
- Uses **stratified sampling** to maintain class distribution in subsets for clustering.

---

## Evaluation Metrics
- **Adjusted Rand Index (ARI):** Measures the similarity between predicted clusters and true labels, adjusted for chance.  
- **V-measure:** Combines cluster **homogeneity** and **completeness**.  

Both metrics help assess how well clustering aligns with actual categories.

---

## Visualizations

### Cluster Centroids
- Average image of each cluster shows the "prototype" of items grouped together.  

### Sample Images per Cluster
- Displays up to **5 images per cluster** with their true labels for visual evaluation.  


---

## Summary
- **K-Means** effectively groups clothing items by pixel similarity.  
- **Agglomerative clustering** produces similar results on a smaller subset.  
- Visual and metric evaluations show the power of unsupervised learning for high-dimensional image data.

---

## Dependencies
- Python 3.8+
- `numpy`
- `matplotlib`
- `scikit-learn`

---
