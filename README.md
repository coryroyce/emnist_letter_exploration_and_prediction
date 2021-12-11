# Explore EMNIST Letter Dataset with Prediction 

Explore the EMNIST letter dataset with various dimensionality reduction techniques and visualizations, and then create an ML model to predict handwritten letters.

# Project Overview
1. Load and select subset of EMNIST Letter dataset
1. Apply various dimensionality reduction techniques with visualizations
1. Create an ML model for prediction
1. Take hand drawn user inputs to create live predictions
1. Visualize prediction bar charts
1. Create interactive web app deployment

# Loading EMNIST Dataset
When exploring various was to import the EMNIST dataset we came across a pre-made Python library called [emnist](https://pypi.org/project/emnist/) which made loading the various sets of data into our project straight forward and simple. After a few custom functions we were able to generate quick visualizations of the letters along with their labels.

![Letter Data Visualization with Label]()



# Reference

## Data Set References

[Original EMNIST Paper](https://arxiv.org/pdf/1702.05373.pdf)

EMNIST dataset: https://www.nist.gov/itl/iad/image-group/emnist-dataset

Direct download: http://www.itl.nist.gov/iaui/vip/cs_links/EMNIST/gzip.zip

Cohen, G., Afshar, S., Tapson, J., & van Schaik, A. (2017). EMNIST: an extension of MNIST to handwritten letters. Retrieved from http://arxiv.org/abs/1702.05373

Importing and formatting Image data inspired by [ArangurenAndres/EMNSIT-Image-classification](https://github.com/ArangurenAndres/EMNSIT-Image-classification/blob/master/cognition_project.ipynb)

Mapping and original file reference [Website](https://www.kaggle.com/crawford/emnist/version/1?select=emnist-balanced-mapping.txt)

## Data Reduction References

Parts of the visualization nad PCA were inspired by [Rahul228646's Kaggle notebook](https://www.kaggle.com/rahul228646/pca-mnist)

Example Data Visualizations for Images from [Kaggle Notebook](https://www.kaggle.com/parulpandey/visualizing-kannada-mnist-with-t-sne)

## Classification Reference

Image Classification in 10 Minutes with MNIST Dataset [Article](https://towardsdatascience.com/image-classification-in-10-minutes-with-mnist-dataset-54c35b77a38d)

How to Develop a CNN for MNIST [Article](https://machinelearningmastery.com/how-to-develop-a-convolutional-neural-network-from-scratch-for-mnist-handwritten-digit-classification/)