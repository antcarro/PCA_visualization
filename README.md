# PCA_visualization
Files in this folder are developed with the .ipynb notebook. 

## Abstract 
In this folder, you'll find the visualizations that I used in a presentation to DePaul's Undergraduate Math Club demonstrating the PCA algorithm on a large, and importantly *visual* dataset. The MNIST dataset is a collection of tens-of-thousands of images of single-digit, hand-written integers. It is widely considered the "Hello World" exercise of machine learning, regression, classification problems. The goal of PCA here is to allow compression of these 28x28 pixel images (encoded as vectors in 784 dimensional space) in smaller-dimensional space. PCA works by finding candidate vectors, which are Eigenvectors of the variance-covariance matrix, so that when you project the dataset into the subspace spanned by these vectors, you maintain as much variance as possible. The idea is quite simple: variance is difference, so if you want to still be able to classify elements, you want to maintain distinguishing features. 

## Files
Aside from the .ipynb file, which lays out all of the code used to produce visualizations, you'll find various .pdf files containing these visualizations. I tend to enjoy the [Eigenimages.pdf](../blob/master/Eigenimages.pdf) file, which shows many of the first 50 of these Eigenvectors, redrawn as images. The first tells us that the most defining characteristic that we can choose is how close to a circle the image appears. This make sense: the digits 0,2,3,6,8,9 would tend to have higher similarity to a circle, while 1,4,5,7 arguably have lower similarity. Meanwhile, "Eigenimage 44" seems to be measuring very fine differences. 

In addition, you'll see the graph [Prediction vs. Components](../blob/master/Predictions%20versus%20components.pdf) which shows how accurate a simple multi-class logistic classifier can be when trained on the compressed images, as a function of how high-dimensional the compressed space can be. 

For fun, I tried to animate a 4 being reconstructed from the components, one-by-one, which you can download in [Reconstruction of 4](../blob/master/test_animation.mp4).
