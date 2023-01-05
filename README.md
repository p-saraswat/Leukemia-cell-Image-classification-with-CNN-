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
*1. Baseline CNN Model*

A baseline Convolutional Neural Network (CNN) is a simple model that can be used as a starting point for developing more complex and accurate models. A baseline model is typically a model that is easy to implement and has reasonable performance, but is not necessarily the best possible model for a given task.

A baseline CNN model might have the following characteristics:
- A small number of layers (e.g., 2-3 convolutional layers and 1-2 fully connected layers)
- A small number of filters in each convolutional layer (e.g., 8-16 filters)
- A small kernel size in the convolutional layers (e.g., 3x3 or 5x5)
- A simple activation function (e.g., ReLU)
- A small batch size (e.g., 32 or 64)
- A simple optimization algorithm (e.g., stochastic gradient descent)
The goal of using a baseline model is to establish a reference point that can be used to compare the performance of more complex models. By comparing the performance of a more complex model to the performance of a baseline model, it is possible to determine whether the added complexity of the model is justified by the improvement in performance.




*2. Inception Model*

An Inception model is a type of Convolutional Neural Network (CNN) architecture that was introduced in the paper "Going Deeper with Convolutions" by Christian Szegedy et al. It was developed to improve upon the traditional CNN architectures that were prevalent at the time, and it has been influential in the field of deep learning.
The main idea behind the Inception model is to use a combination of convolutional layers, pooling layers, and auxiliary classifiers to build a more efficient and powerful CNN. The Inception model is characterized by its use of a "module" that consists of multiple branches, each of which consists of a different type of layer. These branches are then concatenated and the results are fed into the next layer.
One of the key features of the Inception model is its use of dimensionality reduction through the use of 1x1 convolutional filters, which are used to reduce the number of channels in the input tensor. This allows the model to be more computationally efficient, as it reduces the number of parameters that need to be learned.
Overall, the Inception model has been successful in achieving state-of-the-art results on a variety of image classification tasks, and it has been widely adopted in the field of deep learning.

*3. Residual Net Model*

A Residual Network (ResNet) is a type of Convolutional Neural Network (CNN) designed to address the problem of vanishing gradients in deep networks. In a deep neural network, as the number of layers increases, it becomes increasingly difficult to train the network due to the vanishing gradients problem, which refers to the issue of gradients of the weights with respect to the loss becoming smaller and smaller as they are backpropagated through the layers. This can make it difficult for the network to learn and improve.
ResNets address this issue by using skip connections, or shortcut connections, that allow the gradient to bypass one or more layers. These skip connections are used to add the input of a layer to the output of a layer that is several layers deeper in the network. This helps to alleviate the vanishing gradients problem, as it allows the gradient to be directly backpropagated to earlier layers in the network.
The main idea behind ResNets is that by adding these skip connections, it is possible to train much deeper networks without the performance degradation that usually occurs when the network becomes very deep. This has allowed ResNets to achieve state-of-the-art results on a variety of tasks, including image classification, object detection, and semantic segmentation.






## Best Model's performance
Since this is a classification task, we are using accuracy to evaluate the model performance and the following are the accuracies of different models explored
1. Base Model accuracy  =  56%
2. Inception Model = 78%
3. Resnet Model = 82%

Further the model's accuracy could be improved by using Keras's inbuilt ResNet model, which has 50 trained layers.


