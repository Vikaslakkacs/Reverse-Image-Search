# Reverse-Image-Search

This process is similar to image recognition where an input image is provided and output images similar to input images are presented.
### We integrate deep learning and Nearest Neighbors algorithm for detection of similar images.
Deep Learning: We use Pre-trained models (custom models can also be used) to calculate the weights.
Nearest Neighbors: We use NN to pick the best n number of similar images just as input images.

## Applications: Google is using this process to pickup input images and display similar kind of images. Eg: For searching similar kind of furniture where a user has seen and captured an image, Look alike faces etc.,
### Deep learning:
We use ResNet50 in the process for calculation of weights and create features for all the images by predicting the images of same dataset and get the normalisation form of the fetures. Store it in form of pickle for future purposes.
### Nearesst neighbors:
We take the features of the dataset and train NN with the dataset. Later we will pass input image and predict the likely outcomes.
We later use PCA for dimensionality reduction for speed and imporvement in accuracy and predict the likely images.

There are many algorithms where we can use for Nearest Neighbors like Brute force, Annoy, Flann, NGT, Faiss etc., but here as a classical process we are considering brute force algorithm

In the End, we will plot with TSNE all the likely images in the dataset in 2-d format.
