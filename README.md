# Melanoma Detection Assignment


## Table of Contents
* [General Info](#general-information)
* [Contents](#contents)
* [Technologies Used](#technologies-used)
* [Steps performed](#Steps-performed)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
- This repository contains the code for Melanoma Detection.
- Problem Statement
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


- Dataset used: The dataset consists of images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC).

The data set contains the following diseases:

Actinic keratosis
Basal cell carcinoma
Dermatofibroma
Melanoma
Nevus
Pigmented benign keratosis
Seborrheic keratosis
Squamous cell carcinoma
Vascular lesion

## Contents
- Notebook: AnishVA_nn.ipynb

## Steps Performed
Following steps were perfomed as part of the project pipeline
- Reading and Understanding the Data
- Dataset Creation: Creation of train & validation dataset from the train directory with a batch size of 32. Also, image resized to 180*180.
- Visualising the Data
- Model Building & training: Creation of CNN model, rescale images to normalize pixel values between (0,1), Choose an appropriate optimiser and loss function for model training, Train the model for 20 epochs
- Chose an appropriate data augmentation strategy (Image Generator) to resolve underfitting/overfitting 
- Model Building & training on the augmented data 
- Examine the current class distribution in the training dataset
- Handling class imbalances: Rectify class imbalances present in the training dataset with Augmentor library
- Model Building & training on the rectified class imbalance data



## Conclusions
Based on the model metrics, here are the inferences.
- With initial CNN model there was overfit observed
- Used Image generator but model performance did not improve
- Used augmentor to rebalance the data set and added more convultion layer, drop out. Its observed that model accuracy has improved.
    

For more details, refer to AnishVA_nn.ipynb


## Technologies Used
- Keras
- Matplotlib
- Python
- tensorflow
- augmentor
- imagegenerator



## Contact
Created by [@anishnairva] - feel free to contact me!
