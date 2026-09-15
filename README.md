# Retinal OCT Image Classification using SVM & K-Means

Programming Language: Python

This mini project uses ML techniques to classify retinal Optical Coherence Tomography (OCT) images into four categories: Choroidal Neovascularization (CNV), Diabetic Macular Edema (DME), Drusen and Normal Retina.

*How it works?*

OCT Images -> Converts images to greyscale -> Resizes to 128 × 128 -> Normalizes pixel intensities -> Flattens images into feature vectors -> Standardizes features -> Applies PCA for dimensionality reduction -> Classifies images using SVM -> Evaluates using accuracy and confusion matrix -> Applies K-Means clustering for retinal layer segmentation

*Why SVM?*

Support Vector Machine works well with high-dimensional data and can capture non-linear patterns using the RBF kernel. Here, PCA is used before classification to reduce the feature space and retain the most significant information.

*Why K-Means?*

K-Means is an unsupervised ML algorithm that groups pixels with similar intensity values. It is used here to explore retinal intensity patterns and visualize different retinal layers in an OCT image.

*Results*

* Training Accuracy: **95.08%**
* Testing Accuracy: **51.25%**

The large accuracy gap indicates significant overfitting, showing that the current raw pixel + PCA approach has limited generalization for retinal OCT classification.

Dataset: Labelled Optical Coherence Tomography (OCT) for Classification - Mendeley Data
