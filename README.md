
# Myntra Thrift

## Overview

This is our proposed idea for a thrift store for the Myntra HackerRamp We for She competition. Thrift shopping has emerged as a source of sustainable fashion. Along with the reduced environmental impact of buying second-hand clothing, it also caters to the desire of owning luxury clothing at a fraction of the cost of new clothing.
# Our Proposed Solution 
<img src="https://github.com/user-attachments/assets/80daa3c7-1a59-4173-855d-ba682522e92c" alt="Thrift Store for Myntra" width="800"/>


## Proposed Models

### 1. Fashion Captioning Model

#### Dataset
The dataset for this model can be found [here](https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/data).

#### Model Description
The fashion captioning model is based on a large input dataset. The model features are extracted through a Convolutional Neural Network (CNN), then passed through a transformer encoder-decoder and trained using a large-scale fashion image and description dataset. This model is designed to generate automatic captions for given input images.
#### Result
<img src="https://github.com/user-attachments/assets/320df869-8ab2-413c-ac44-2c6c89275597" alt="Thrift Store for Myntra" width="800"/>


### 2. Price Prediction Model

#### Dataset
The dataset for this model can be found [here](https://www.kaggle.com/datasets/justinpakzad/vestiaire-fashion-dataset).

#### Model Description
The price prediction model is designed to suggest an appropriate price for second-hand clothing. Given inputs like clothing type, material quality, Brand and expected price, the model predicts a suitable price. The model is trained using a second-hand price prediction dataset.

#### Model inputs and Features
The input features for the price suggestion model are mapped to the user queries in the thrift store app accordingly.


| **Input Feature**           | **Question**                                                                 | **Explanation**                                                                                                           |
|-----------------------------|------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| `seller_price`              | What is the price that you bought it for?                                     | This is the price at which the seller originally purchased the product.                                                   |
| `product_material`          | What is the material of the product?                                          | The material composition of the product (e.g., cotton, polyester).                                                        |
| `product_category`          | Tell us the product category (bottom, top, others)                            | The category to which the product belongs (e.g., bottom wear, top wear, others).                                          |
| `product_gender_target`     | What is the gender target for this product?                                   | The gender for which the product is intended (e.g., male, female, unisex).                                                |
| `product_color`             | What is the color of the product?                                             | The color of the product.                                                                                                 |
| `product_condition`         | How many times have you worn this product?                                    | The current condition of the product, mapped to how many times it has been worn (e.g., new, like new, used).              |
| `brand_name`                | What is the brand name of your product?                                       | The brand under which the product is sold.                                                                                |
| `product_type`              | What is the product type?                                                     | The specific type of product within the category (e.g., jeans, t-shirt).                                                  |
| `product_season`            | Which season is the most suitable for this product?                           | The season in which the product is best suited to be worn (e.g., summer, winter).                                         |
| `warehouse_name`            | What is your address?                                                         | The address of the customer.                                                                                              |



The expected price provided by the user will be double-checked with the price predicted by the model. If the expected price falls within a safe range, it will be approved.


