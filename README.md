# Customer Segmentation of German Bank Credit Data

## Project Overview
This project uses unsupervised machine learning techniques to segment customers in the German Bank Credit dataset. By clustering similar customer profiles, banks can gain insights into financial behavior, risk levels, and credit allocation patterns.

## Dataset
The dataset includes the following features:

- Age
- Sex
- Job
- Housing
- Saving accounts
- Checking account
- Credit amount
- Duration
- Purpose

**Note:** The dataset does not include target labels. The analysis is purely unsupervised.

Source: [Kaggle German Bank Credit Data](https://www.kaggle.com/datasets/kamaumunyori/german-bank-credit-data)

## Methodology

1. **Data Preprocessing**
   - Handle missing values in `Saving accounts` and `Checking account` using credit amount-based imputation.
   - Encode categorical features (`little < moderate < quite rich < rich`) using ordinal encoding.
   - One-hot encode other categorical features like `Sex`, `Housing`, and `Purpose`.
   - Scale numeric features (`Age`, `Credit amount`, `Duration`) for clustering.

2. **Clustering**
   - **KMeans++**: Groups customers into distinct clusters based on financial features.
   - **Hierarchical Clustering**: Provides a dendrogram and cluster assignments for comparison.

3. **Dimensionality Reduction**
   - **PCA** used to reduce features to 2D for visualization.
   - Clustered customers visualized in 2D to identify patterns and relationships.

## Tools & Libraries
- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
- scipy


