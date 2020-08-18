# MRI-Brain-Tumor-Detection

### Brain tumor
A brain tumor occurs when abnormal cells form within the brain

Building a detection model using a convolutional neural network in Tensorflow & Keras.


About the data:
The dataset contains 2 folders: 
yes and no which contains 253 Brain MRI Images. 
The folder yes contains 155 Brain MRI Images that are tumorous and the folder no contains 98 Brain MRI Images that are non-tumorous.


### Data Augmentation:

Why did I use data augmentation?

Since this is a small dataset, There wasn't enough examples to train the neural network. Also, data augmentation was useful in taclking the data imbalance issue in the data.
so I apply data arugumentation using ImageDataGenerator 

### Data Preprocessing

For every image, the following preprocessing steps were applied:

Resize the image to have a shape of (224, 224, 3)=(image_width, image_height, number of channels): because images in the dataset come in different sizes. So, all images should have the same shape to feed it as an input to the neural network.

Apply normalization: to scale pixel values to the range 0-1.


### Data Split:

The data was split in the following way:

* 60% of the data for training.
* 20% of the data for validation.
* 20% of the data for testing.


### Neural Network Architecture








