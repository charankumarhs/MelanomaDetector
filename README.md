# Multiclass classification model using a custom convolutional neural network in TensorFlow. 
This is part of convolutional Neural Network demonstartion from the skills gained during the course study using dataset consists of 2239 training images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC).

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

#### Essentially, the model should categorize the images into the following 9 categories accurately,
    1. Actinic keratosis
    2. Basal cell carcinoma
    3. Dermatofibroma
    4. Melanoma
    5. Nevus
    6. Pigmented benign keratosis
    7. Seborrheic keratosis
    8. Squamous cell carcinoma
    9. Vascular lesion 

## Conclusions

1. The dataset has got class imabalance and the generic CNN model we built is overfitting. We can see that the accuracy of the model with training dataset is increasing over time with each epoch, reaching an accuracy of 85%+, whereas the accuracy of the validation dataset stalls around 50-55%. Furthermore, the difference between accuracy of training and validation dataset is ~30%+, which is a huge difference and the model is clearly Overfitting. The overfitting in this case is most likely due to less number of images in the dataset we are giving to the model for learning and the model could be learning from noise or unwanted data.
2. The model built with data augmentation to fix the problem of overfitting helped in reducing the overfitting of the model but the model accuracy is coming around ~60%, which is not great.
3. Rectified the class imbalance using Augmentor and then built a model with good amount of experimentation of the model with choosing activation functions, addring dropout layers, adding batch normalization, choosing the optimizers, which worked out well. A model with ~86% accuracy with validation data set is built.


## Technologies Used
- library -  pandas  version  1.5.3
- library -  numpy  version  1.23.5
- library -  seaborn  version  0.12.2
- library -  matplotlib  version  3.7.1
- library -  seaborn  version  0.12.2
- library -  PIL  version  9.4.0
- library -  tensorflow  version  2.12.0
- library -  keras.api._v2.keras  version  2.12.0
- library -  cv2  version  4.7.0
- library -  google.colab  version  0.0.1a2
- library -  Augmentor  version  0.2.12

## Acknowledgements

- This project was done as part of the Machine Learning and Artificial Intelligence Master Degree program by upGrad in asssociation with IIIT-B and LJMU.


## Contact
Created by [@charankumarhs] - feel free to contact me!
