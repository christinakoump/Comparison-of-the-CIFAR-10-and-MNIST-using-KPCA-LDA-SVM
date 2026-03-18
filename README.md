# Comparison-of-the-CIFAR-10-and-MNIST-using-KPCA-LDA-SVM
MNIST & CIFAR-10 Unsupervised Clustering

This repository explores unsupervised machine learning pipelines for image classification using the MNIST and CIFAR-10 datasets. The project focuses on how dimensionality reduction can enhance clustering performance in high-dimensional feature spaces.
Pipeline:

    Preprocessing: Normalizes pixel values to a [0,1] range and flattens images into 1D vectors.

    Dimensionality Reduction: Uses t-SNE to project high-dimensional data into 2D components, preserving local structures for better grouping.

    Clustering: Applies Spectral Clustering to the 2D projections to identify patterns without using labels.

    Classification: Assigns test data to clusters based on the nearest Euclidean distance to calculated cluster centers.

    Evaluation: Measures quality using the Adjusted Rand Index (ARI), accuracy, and confusion matrices.

Required libraries: numpy, scikit-learn, tensorflow (for data loading),  matplotlib


Results:

    MNIST: Shows high clustering purity due to the distinct shapes of handwritten digits.

    CIFAR-10: Proves more challenging as RGB object intensities vary significantly within the same class.
