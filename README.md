# Machine Learning in Medicine and Healthcare

Project contains application of various machine learning methods on medicine and healthcare related problems.

## Description

The project contains Jupyter Notebooks with Python code and printed outputs. Each `hw` folder contains the data and relevant IPython Notebook for analysis.

`scikit-learn`, `pandas`, `numpy`, `matplotlib`, and `keras` packages were used for analysis and visualization, with additional utility packages to handle compressed files and batch downloads of data from various public access APIs.

- `hw1` folder contains code demonstrating a single file download from the 'files' endpoint of gdc.cancer.gov API, as well as some exploratory analysis on RNE-seq data for a single sample.
- `hw2` folder contains the code for batch downloading from GDC API, concatenating multiple samples of RNE-seq data. Later, the RNE-sequences are clustered and these clusters are visualized using t-SNE for dimensionality reduction, and `scikit-learn` implementations of K-Means, DBSCAN, and Agglomerative Clustering for unsupervised learning.

# Author

Egemen Pamukcu ([LinkedIn](https://linkedin.com/in/egemenpamukcu))
