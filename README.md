# Image-Colorisation-Project
## Table of Contents
* [Description](#Description "Goto Description")
* [Autoencoder](#Autoencoder "Goto Autoencoder ")
* [Resnet 18 Gray](#Description "Goto Description")
* [LAB Color Space](#Description "Goto Description")
* [Model Architecture](#Description "Goto Description")
* [Results](#Description "Goto Description")
## Description
In this project I have used autoencoder to train the network to colorise the grayscale images.
## Autoencoder 
I have used autoencoder in this project.Autoencoder is a neural network which is composed of encoder,bottleneck and a decoder.
* Encoder:
An encoder compresses the input data in a latent space representation, generating a new representation of the data that has reduced dimensionality.
* Bottleneck:
A module that contains the compressed knowledge representations and is therefore the most important part of the network.
* Decoder:
 A module that helps the network“decompress” the knowledge representations and reconstructs the data back from its encoded form. The output is then compared with a ground truth.
## Resnet 18 Gray
The reason why we use resnet is Deep neural networks are hard to train as their depth increases. This increase in depth comes with many problems. Residual Networks or ResNets are a solution to such problems
In this project I have used Resnet 18 Gray which is a pretrained Convolutional neural network that is 18 layers deep,but I have used just first 6 layers of this network.
## LAB Color Space
I have used LAB Color Space in this project as by separating out the gray-scale component, the neural network only has to learn the remaining two channels for colorization. This reduces size of the network and speed of convergence.

## Model Architecture
![Arcitecture](https://cdn.discordapp.com/attachments/993239385891942421/1030118698071101500/unknown.png)
* Batch Size:60
* Input Image Size:(256,256)
* Loss Fuction:MSE Loss
* Optimizer:Adam with learning rate as 0.001

## Results
![results](https://cdn.discordapp.com/attachments/993239385891942421/1031769458508841000/unknown.png)


![result](https://user-images.githubusercontent.com/107758088/197851113-7244c3cd-4d10-4d5f-8c2c-1825959e6e8e.png)

