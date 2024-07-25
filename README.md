# Solar Farm Detection from Satellite Images

This project aims to detect and delineate solar farms from satellite images using a convolutional neural network (CNN). The model is capable of processing images in multiple formats and provides a binary classification indicating the presence of a solar farm. If a solar farm is detected, the model can also extract the solar farm from the image.

## Table of Contents
- [Overview](#overview)
- [Data Acquisition and Preparation](#data-acquisition-and-preparation)
- [Model Development](#model-development)

## Overview
The primary goal of this project is to utilize satellite images to detect and delineate solar farms. The model is trained to distinguish between images containing solar farms and those without.

## Data Acquisition and Preparation
- **Data Collection:** Satellite images of solar farms and non-solar areas were collected from various sources.
- **Data Annotation:** Images were labeled and organized into two categories: `solar_farm` and `non_solar_farm`.
- **Data Preprocessing:** Images were resized to 150x150 pixels and normalized. The data was then split into training and validation sets.

## Model Development
A convolutional neural network (CNN) was designed and implemented using TensorFlow and Keras. The model architecture includes multiple convolutional layers, batch normalization, max pooling, and global max pooling, followed by a dense output layer with a sigmoid activation function.

### Key Components:
- **Convolutional Layers:** Extract features from images.
- **Batch Normalization:** Improves training speed and stability.
- **Max Pooling:** Reduces the dimensionality of feature maps.
- **Global Max Pooling:** Downsamples feature maps to a single vector.
- **Dense Layer:** Outputs a binary classification indicating the presence of a solar farm.

