# CSCI E-89 Deep Learning: Multi-Class Brain Tumor Classification Using Convolutional Neural Networks

Cristina Kennedy, RN, BSN

December, 2025

# Data set
https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset/data

## Abstract
This project proposes a custom-built convolutional neural network model trained from scratch to distinguish between normal brain scans and gliomas, meningiomas and pituitary tumors on brain MRI images. The primary interest is to close the gap in care where radiologists miss brain cancers on MRIs, which creates a significant opportunity for AI systems to serve as a secondary reader.

## Overview of steps

### Data loading and preparation
Data was retrieved from Kaggle: Brain Tumor MRI Dataset. Tensorflow.keras.preprocesing.image.ImageDataGenerator and flow_from_dataframe were used to load and preprocess the data.

### Model Architecture and Training
Custom-built convolutional neural network (sequential) consisting of four convolutional layers and max-pooling layers, one dropout layer and two dense layers. The SoftMax classifier was paired with cross-entropy loss function. Trained the CNN model on 50 number of epochs. 

### Model Deployment
Deployed the project with Flask by hosting a web server that bridges the gap between users and the deep learning model.

The file "index.html" needs to be moved to the subfolder ./templates/index.html
Note that you will have to interrupt the kernel or Jupyter to stop the web server execution.

## Results
The model achieved an accuracy of 97%, 97% precision and 97% recall. A customized CNN achieved high performance, but arguments can be made that the model can be improved by using transfer learning.
