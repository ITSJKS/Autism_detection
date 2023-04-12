# Autism Detection Project

This project is aimed at detecting autism in children using deep learning models. We have used VGG16 and EfficientNet models to classify whether a child has autism or not based on MRI brain images.

## Dataset

We have used a dataset which we found on kaggle which contains about 3000 images of autistic and non autistic children.

## Preprocessing

We preprocessed the images by resizing them to 224x224 pixels, converting them to grayscale, and normalizing the pixel values. We also split the dataset into training, validation, and test sets with a ratio of 70:15:15.

## Models

We have used two deep learning models to classify the MRI images:

* VGG16 - A convolutional neural network (CNN) architecture that consists of 16 layers.
* EfficientNet - A CNN architecture that uses a novel compound scaling method to achieve state-of-the-art performance with fewer parameters and faster training times.

We trained both models on the training set and evaluated their performance on the validation set.
* EfficientNet model based on media pipe - we cropped the images of our previous dataset based on important face point in the faces. We then trained our model based on it which helped us to increase our accuracy to 90%.

## Results

After training and evaluating both models, we found that the EfficientNet model outperformed the VGG16 model with an accuracy of 85% compared to 80%.

## Dependencies

* Python 3.6+
* TensorFlow 2.0+
* Keras 2.2+
* NumPy
* Matplotlib
* MediaPipe

## Conclusion

In this project, we have shown that deep learning models can be used to accurately detect autism in children using MRI brain images. Our results demonstrate that the EfficientNet model outperforms the VGG16 model in terms of accuracy.
