# Skin-Cancer-Detection
Skin-Cancer (Malignant vs. Benign) Detection using Deep-CNN and Hyperparameter tuning using keras-tuner

## Overview
In this work, we address the problem of skin cancer classification using convolutional neural networks. A lot of cancer cases early on are misdiagnosed leading to severe consequences including the death of patient. Also there are cases in which patients have other problems and doctors interpret it as skin cancer. This leads to unnecessary time and money spent for further diagnosis. In this work, we address the above problems using deep cnn neural networks.

## Sample images
### Benign image sample
![benign](https://user-images.githubusercontent.com/90151852/133253297-59a52eb7-42c4-45bf-9029-27e8213896f1.png)

### Malignant image sample
![malignant](https://user-images.githubusercontent.com/90151852/133253503-5ae2481e-d736-4e95-8044-076ffef61813.png)

## Plot
### Losses plot
![skin loss](https://user-images.githubusercontent.com/88196035/135041518-8401ff93-db4a-4c19-80c4-57efd2277fe3.png)

### Accuracy plot
![skin acc](https://user-images.githubusercontent.com/88196035/135041537-4765fe9f-3573-443c-9c7d-e18603c23a13.png)

## Result
### Confusion matrix
array([[304,  56],

       [ 36, 264]])
       
### Classification report
              precision    recall  f1-score   support

           0       0.89      0.84      0.87       360
           1       0.82      0.88      0.85       300

    accuracy                           0.86       660

## Image Manipulation (ImageDataGenerator)
Its usually a good idea to manipulate the images with rotation, resizing, and scaling so the model becomes more robust to different images that our data set doesn't have. We can use the ImageDataGenerator to do this automatically for us.

##  Hyperparameter Tuning using Keras-Tuner
For Hyperparameter Tuning using Keras-Tuner, we define a function so that we can perform hyperparameter tunning and improve our model but it takes usually more time to tune our model so that after finding hyperparameter we can Fill the Values and steps for testing of a model and then retrieve the best model among them.

## Dataset
This dataset contains a balanced dataset of images of benign skin moles and malignant skin moles.The data consists of two folders with each 1800 pictures (224x244) of the two types of moles.

The dataset can be downloaded here: https://www.kaggle.com/fanconic/skin-cancer-malignant-vs-benign
