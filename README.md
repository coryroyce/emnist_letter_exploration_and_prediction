# Explore EMNIST Letter Dataset with Prediction 

Explore the EMNIST letter dataset with various dimensionality reduction techniques and visualizations, and then create an ML model to predict handwritten letters.

# Project Overview
1. EMNIST Letter Dataset
1. Dimensionality Reduction Techniques
1. ML Model
1. User Application
1. Web Deployment

# Loading EMNIST Letter Dataset
When exploring various was to import the EMNIST dataset we came across a pre-made Python library called [emnist](https://pypi.org/project/emnist/) which made loading the various sets of data into our project straight forward and simple. After a few custom functions we were able to generate quick visualizations of the letters along with their labels.

![Letter Data Visualization with Label](https://github.com/coryroyce/emnist_letter_exploration_and_prediction/blob/main/reference/labeled_image_A.png)

# Dimensionality Reduction Techniques
During the data exploration stage we applied several dimensionality reduction techniques to better visualize how the letter images could be clustered together. The highlights are PCA (Principal Component Analysis) which is a good baseline technique and UMAP (Uniform Manifold Approximation and Projection) which provide clearer clusters and better separation. Images shown below and full code can be found in the [dev_notebooks folder](https://github.com/coryroyce/emnist_letter_exploration_and_prediction/blob/main/dev_notebooks/Letter_Exploration_and_Classification_V04.ipynb).

![PCA of Letters](https://github.com/coryroyce/emnist_letter_exploration_and_prediction/blob/main/reference/PCA_of_letters.png)

![UMAP of Letters](https://github.com/coryroyce/emnist_letter_exploration_and_prediction/blob/main/reference/UMAP_of_letters.png)

# ML Model
After creating a few different versions of a Tensorflow Deep Neural Net we ultimately used an architecture that did well in a [Kaggle competition](https://www.kaggle.com/cdeotte/25-million-images-0-99757-mnist) with the 0-9 MNIST digit data set.

![Model Architecture - Image from cdeotte/25-million-images-0-99757-mnist](https://github.com/coryroyce/emnist_letter_exploration_and_prediction/blob/main/reference/model_architecture_diagram.png)

# User Application
To create an interactive experience for users to draw handwritten digits and provide model prediction in real time, we used [Streamlit](https://streamlit.io/) to create our [front end application](https://github.com/coryroyce/emnist_letter_exploration_and_prediction/tree/main/streamlit_application). This demo can easily be run in out [Streamlit_App.ipynb](https://github.com/coryroyce/emnist_letter_exploration_and_prediction/blob/main/streamlit_application/Streamlit_App.ipynb) Colab notebook.

![App Example](https://github.com/coryroyce/emnist_letter_exploration_and_prediction/blob/main/reference/app_demo_image.png)

# Web Deployment

To make our Letter drawing prediction application as accessible as possible we created a self contained web app and deployed it using [Heroku](https://dashboard.heroku.com/apps) which can be found in the [heroku_app folder](https://github.com/coryroyce/emnist_letter_exploration_and_prediction/tree/main/heroku_app).

[Initial Demo Link](https://letter-prediction.herokuapp.com/)

# Contributors
coryroyce


# Reference

Live Demo Video: https://youtu.be/wI2hDtuRbUw

Project PPT Link: https://docs.google.com/presentation/d/1svfLKvYqRFLc2mmICwIRXpxxdTbY63B64NXi0cnEuyM/edit#slide=id.g106ebbdb28d_0_51

Project Report Link: https://docs.google.com/document/d/1S3f0IWZUfYTdzhxm7Hy8ESF2y3pgSkd_AvRUsdQ6OI0

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

Kaggle Competition with MNIST 0-9 digits [Article](https://www.kaggle.com/cdeotte/25-million-images-0-99757-mnist)
