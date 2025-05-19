# Image Caption Generator

## Overview

This repository contains code for an image caption generation system using deep learning techniques. The system leverages a pretrained VGG16 model for feature extraction and a custom captioning model which was trained using LSTM for generating captions. The model is trained on the Flickr8k dataset using an attention mechanism to improve caption quality.

The key components of the project include:

- Image feature extraction using a pretrained VGG16 model (Consider using MobileNetV2 for memory efficiency)
- Caption preprocessing and tokenization
- Custom captioning model architecture with attention mechanism
- Model training and evaluation
- Streamlit app for interactive caption generation

## About the Dataset

The [Flickr8k dataset](https://www.kaggle.com/adityajn105/flickr8k) is used for training and evaluating the image captioning system. It consists of 8,091 images, each with five captions describing the content of the image. The dataset provides a diverse set of images with multiple captions per image, making it suitable for training caption generation models.

Download the dataset from [Kaggle](https://www.kaggle.com/adityajn105/flickr8k) and organize the files as follows:

- flickr8k
  - Images
    - (image files)
  - captions.txt
## Scope of Work
Data Collection and Preprocessing:

-Utilize the Flickr8k Dataset, which contains a diverse collection of images with corresponding captions.
-Preprocess the images to standardize size, format, and quality, and tokenize the captions.
Feature Extraction:

-Leverage the VGG16 model, pretrained on ImageNet, to extract high-level features from images.
-Fine-tune the VGG16 model to enhance feature representation.
Caption Generation Model:

-Develop an LSTM-based RNN to generate captions from the extracted image features.
-Train the model on the preprocessed image-caption dataset, integrating VGG16 and LSTM.
#Evaluation:

-Evaluate the model’s performance using the BLEU score to measure the quality of generated captions.
-Optimize the model for better accuracy and faster inference times.

