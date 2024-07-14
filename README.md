
# Myntra Thrift

## Overview

This is our proposed idea for a thrift store for the Myntra HackerRamp We for She competition. Thrift shopping has emerged as a source of sustainable fashion. Along with the reduced environmental impact of buying second-hand clothing, it also caters to the desire of owning luxury clothing at a fraction of the cost of new clothing.
# Our Proposed Solution 
<img src="https://github.com/user-attachments/assets/80daa3c7-1a59-4173-855d-ba682522e92c" alt="Thrift Store for Myntra" width="400"/>


## Proposed Models

### 1. Fashion Captioning Model

#### Dataset
The dataset for this model can be found [here](https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/data).

#### Model Description
The fashion captioning model is based on a large input dataset. The model features are extracted through a Convolutional Neural Network (CNN), then passed through a transformer encoder-decoder and trained using a large-scale fashion image and description dataset. This model is designed to generate automatic captions for given input images.

### 2. Price Prediction Model

#### Dataset
The dataset for this model can be found [here](https://www.kaggle.com/datasets/justinpakzad/vestiaire-fashion-dataset).

#### Model Description
The price prediction model is designed to suggest an appropriate price for second-hand clothing. Given inputs like clothing type, material quality, Brand and expected price, the model predicts a suitable price. The model is trained using a second-hand price prediction dataset.

