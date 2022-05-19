# Image-Classifier
## The main goal of this Project is to create an image classifier from scratch using the Keras package.

## Prerequisites
- Python 3.x

In order to proceed the Project I have used car images, which I downloaded from internet, as object and other random images such as image of mountains, different scene and people as not object.
I have created folder called Image, inside image there is 2 sub folders "Object" and "not object" where car images were placed in object folder, where as other images were present in not object folder.

The classifier will be built in two ways:
- Original dataset present inside Image folder
- Using data augmentation method

#### The splitfolders model is used to split images into train, test and validation set where I have maintained the ratio of 0.625:0.1875:0.1875 to train, validation, and test set so that each set contains 50, 15,15 images from object and not object folders.

## Installing Dependencies
Note: You can skip this step, if you already installed the packages that mentions below. Dependencies are listed in the requirements.txt file

## Necessary Libraires or packages are:-
- TensorFlow
- Keras
- Numpy
- numpy
- Matplotlib

## Process
1. Dataset Verification
2. Dataset Loading and Processing with Image Data Generators
3. Create and Evaluate a Model
4. Report Accuracy on Test Set
Following steps were implemented in the `lab 4.ipynb` File, you can refer this file for comlpete process

### In order to address overfitting I have used `EarlyStopping callbacks` model which prevent model from learning/predicting further if the validation accuracy stops improving.
## Test accuracy in this process is pretty low so, I have also used image data augumentation method, the purpose of the augumentation is to increase range of the training images by transforming it into various stages. In the Augmentation method I have used: rotation range, width_shift_range, height_shift_range, rescale, shear_range,zoom_range,horizontal_flip, and fill mode methods.

## In order to complete this lab I have used folllowing blogs as a references

- https://colab.research.google.com/github/tensorflow/docs/blob/master/site/en/tutorials/images/data_augmentation.ipynb#scrollTo=eR4wwi5Q_UZK
- https://blog.keras.io/building-powerful-image-classification-models-using-very-little-data.html
- https://keras.io/examples/vision/image_classification_from_scratch/

