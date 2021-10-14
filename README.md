# CNN-on-Custom-Images
Implementation of Convolutional neural network on Custom Images

# Dataset

Dataset consists of both train set Images and test set images of CATS and DOGS i.e 2Classes.

Train set- 9,372 Images of DOGS and 9,371 Images of CATS

Test set- 3,127 Images of DOGS and 3,126 Images of CATS

# Preparing the data for the classification task

Each Image in the dataset have different number of pixels. So, we have to bring them to the same size for this task. Identifying the right size is one of the crucial steps.

We can also do few transformations like Cropping, Resizing, Flipping, Rotation on the images to get good generalisation for the model if the images in the dataset have some particular trend.

 Original Image
 ![](https://github.com/Yashwanthkumar11/CNN-on-Custom-Images/blob/master/.ipynb_checkpoints/p1.png)
 
 Random-horizontal-Flip 
 ![](https://github.com/Yashwanthkumar11/CNN-on-Custom-Images/blob/master/.ipynb_checkpoints/p2a.png)
 
 Resized and Center-cropped
 ![](https://github.com/Yashwanthkumar11/CNN-on-Custom-Images/blob/master/.ipynb_checkpoints/p2.png)
 
 Rotated 
 ![](https://github.com/Yashwanthkumar11/CNN-on-Custom-Images/blob/master/.ipynb_checkpoints/p3.png)
 
 After all transormations 
 ![](https://github.com/Yashwanthkumar11/CNN-on-Custom-Images/blob/master/.ipynb_checkpoints/p4.png)

Since implementation is done using pyTorch, we have to convert the pixels array to tensors.

# Model

Used a simple model with 2 convolutional layers, 2 pooling layers, 3 fully-connected layers. Detailed description of the model can be seen in the below image.

![](https://github.com/Yashwanthkumar11/CNN-on-Custom-Images/blob/master/.ipynb_checkpoints/p5.png)

# Training and test accuracies during training

![](https://github.com/Yashwanthkumar11/CNN-on-Custom-Images/blob/master/.ipynb_checkpoints/p6.png)

# Overall accracy on the test data after training
![](https://github.com/Yashwanthkumar11/CNN-on-Custom-Images/blob/master/.ipynb_checkpoints/p7.png)

For the detailed understanding of the working, please go through python notebook file in this repo.



