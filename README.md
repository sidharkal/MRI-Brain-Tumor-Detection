# MRI-Brain-Tumor-Detection

### Brain tumor
A brain tumor occurs when abnormal cells form within the brain

Building a detection model using a convolutional neural network in Tensorflow & Keras.

you can download Dataset From [here](https://www.kaggle.com/navoneel/brain-mri-images-for-brain-tumor-detection) 


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

* 70% of the data for training.
* 15% of the data for validation.
* 15% of the data for testing.


### Neural Network Architecture

![Image](https://www.google.com/search?q=Neural+Network+Architecture+in+Mri+image&tbm=isch&ved=2ahUKEwjm2ISx3aTrAhUSkUsFHc_WA5oQ2-cCegQIABAA&oq=Neural+Network+Architecture+in+Mri+image&gs_lcp=CgNpbWcQAzoECAAQGFDTCFilKmDJK2gAcAB4AIABugGIAZgMkgEEMC4xMJgBAKABAaoBC2d3cy13aXotaW1nwAEB&sclient=img&ei=RcY7X6aiG5KirtoPz62P0Ak&bih=722&biw=1536#imgrc=cek2XEFpDF0LgM.png)








