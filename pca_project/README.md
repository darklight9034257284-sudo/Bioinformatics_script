# <<<<<<< HEAD
# PCA on Gene Expression Data**

# **Overview**


In this project, we explore how Principal Component Analysis (PCA) can help us understand patterns in gene expression data, specifically for breast cancer patients.

Instead of just looking at thousands of genes individually, PCA helps reduce the complexity and lets us visualize meaningful patterns in a simpler way.

 # ****Objective****


The main goals of this project were:

Extract expression levels of two important genes: XBP1 and GATA3

Visualize their relationship using a scatter plot

Apply PCA to reduce dimensions

Project the data onto the first principal component (PC1)

**Dataset**
We used gene expression data from 105 patients, organized into:

class.tsv → Labels (ER+ or ER-)

filtered.tsv.gz → Gene expression values

columns.tsv.gz → Mapping of gene IDs to gene names
What I Did
1. Data Processing
Loaded all datasets using Python

Identified the gene IDs for XBP1 and GATA3

Extracted their expression values for all patients

2. Visualization
Created a scatter plot of XBP1 vs GATA3

Colored points based on cancer type (ER+ / ER-)

This helps visually see if the two groups separate

3. PCA Implementation
Applied PCA on the dataset

Reduced high-dimensional data to 1 principal component (PC1)

Projected samples onto PC1

This shows how well PCA separates the classes

# Results
The scatter plot shows a clear pattern between the two gene expressions

PCA projection highlights separation between ER+ and ER- samples

Even though data is high-dimensional, PCA captures important variation effectively

# PCA-project

PCA on gene expression data.

Usage
-----

Run the analysis script with Python 3. Requirements: pandas, numpy, matplotlib, scikit-learn.

Example:

	python3 pca_project.py


