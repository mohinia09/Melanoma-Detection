# Melanoma Detection using CNN
> To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis. 


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- We will build a multiclass classification model using a custom convolutional neural network in TensorFlow. 
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Using a Sequential CNN using 3 convolution layers with 16, 32 nd 64 filters respectively, the training accuracy and validation accuracy were off by large margins.
The model achieved only around 50% accuracy on the validation set. This was a case of overfitting which had to be resolved.
- Next, we tried an augmentation strategy of random flip, zoom and rotate which resulted in reduction of overfitting problem and the train and validation sets showed a linear increase in accuracy. Hence, the new model is an improvement as compared to the previous model.
- On analysis we found that the dataset has class imbalance. The following classes have min. and max. number of images:
  - "Seborrheic Keratosis" - 58.
  - "Pigmented Benign Keratosis" - 370.
  - ~ 1/3 of the samples belong to the classes "Pigmented Benign Keratosis" and "Basal Cell Carcinoma". </br>
This class imbalance was handled by adding 500 images to each class.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Tensorflow
- Keras
- Numpy
- Pandas
- Matplotlib
- Augmentor


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements


## Contact
Created by [@mohinia09] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
