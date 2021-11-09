# Machine Learning in Medicine and Healthcare

Project contains application of various machine learning methods on medicine and healthcare related problems.

## Description

The project contains Jupyter Notebooks with Python code and printed outputs. Each `hw` folder contains the data and relevant IPython Notebook for analysis.

`scikit-learn`, `pandas`, `numpy`, `matplotlib`, and `keras` packages were used for analysis and visualization, with additional utility packages to handle compressed files and batch downloads of data from various public access APIs.

- `hw1` folder contains code demonstrating a single file download from the 'files' endpoint of gdc.cancer.gov API, as well as some exploratory analysis on RNE-seq data for a single sample.
- `hw2` folder contains the code for batch downloading from GDC API, concatenating multiple samples of RNE-seq data. Later, the RNE-sequences are clustered and these clusters are visualized using t-SNE for dimensionality reduction, and `scikit-learn` implementations of K-Means, DBSCAN, and Agglomerative Clustering for unsupervised learning.
- `hw3`
  - `predicting-tumor`
    - In this notebook I build models that takes RNAseq profiles from matched normal-tumor pairs and classifies the sample as Normal or Tumor. I try to do this task using two different subsets of the feature space: firstly using the complete gene expression data available, and later using only the expressions of protein encoding genes and compare results.
  -  `predicting-drug-response`
      - In this notebook I build two Random Forest models to predict drug response by using data from CTRP study. This data consists of drug response information from 53 drugs tested on hundreds of cell lines. Our dependent variable of interest is an AUC (area under the curve) value where higher values indicate drug sensitivity for a specific cell line. First, I use a Random Forest Regressor to predict an AUC value between 0 and 1. Later, I bin these AUC values into three bins representing Susceptible, Intermediate, and Resistant categories and fit a Random Forest Classifier.
  -  `classifying-cancer-types`
      -  In this notebook I try to classify cancer types based on gene expressions for 5,400 samples. After splitting the data into trainig and testing sets, in order to make computation more feasible, I first reduce the dimensionality of our feature matrix using the PCA algorithm from 60,483 to 1,000. The first 1,000 components explained about 64% of the variance in hte original dataset. I also observed that the accuracy of both traditional and deep learning methods improved with fewer dimensions.
  -  `autoencoder-gene-expressions`
      - In this notebook I build an autoencoder that takes ~19,000 protein encoding gene expression values as input, and encodes it to varying (much smaller) dimensions and then decodes them back to the original width of the input.


# Author

Egemen Pamukcu ([LinkedIn](https://linkedin.com/in/egemenpamukcu))
