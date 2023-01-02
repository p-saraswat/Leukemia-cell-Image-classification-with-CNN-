# Leukemia-classification using CNN 

Acute lymphoblastic leukemia (ALL) is the most common type of childhood cancer and accounts for approximately 25% of the pediatric cancers.

These cells have been segmented from microscopic images and are representative of images in the real-world because they contain some staining noise and illumination errors, although these errors have largely been fixed in the course of acquisition.

The task of identifying immature leukemic blasts from normal cells under the microscope is challenging due to morphological similarity and thus the ground truth labels were annotated by an expert oncologist.

In total there are 15,135 images from 118 patients with two labelled classes:

1. ***Normal cell***

![image](https://user-images.githubusercontent.com/121529081/210246623-9cc0e959-b598-434f-9688-411a339d671b.png)

2. ***Leukemia blast***
![image](https://user-images.githubusercontent.com/121529081/210246335-7eb59369-4e98-4579-9ff3-523f78f2a23a.png)


## Data Citation
Gupta, A., & Gupta, R. (2019). ALL Challenge dataset of ISBI 2019 [Data set]. The Cancer Imaging Archive. https://doi.org/10.7937/tcia.2019.dc64i46r

## Models explored 
1. Baseline CNN Model

2. Inception Model
An Inception model is a type of Convolutional Neural Network (CNN) architecture that was introduced in the paper "Going Deeper with Convolutions" by Christian Szegedy et al. It was developed to improve upon the traditional CNN architectures that were prevalent at the time, and it has been influential in the field of deep learning.

The main idea behind the Inception model is to use a combination of convolutional layers, pooling layers, and auxiliary classifiers to build a more efficient and powerful CNN. The Inception model is characterized by its use of a "module" that consists of multiple branches, each of which consists of a different type of layer. These branches are then concatenated and the results are fed into the next layer.

One of the key features of the Inception model is its use of dimensionality reduction through the use of 1x1 convolutional filters, which are used to reduce the number of channels in the input tensor. This allows the model to be more computationally efficient, as it reduces the number of parameters that need to be learned.

Overall, the Inception model has been successful in achieving state-of-the-art results on a variety of image classification tasks, and it has been widely adopted in the field of deep learning.

3. Residual Net Model

## Best Model's performance

