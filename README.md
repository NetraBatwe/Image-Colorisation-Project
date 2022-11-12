# Image-Colorisation-Project
## Table of Contents
* [Description](#description "Goto Description")
* [Dataset](#dataset "Goto Dataset")
* [Methods](#methods "Goto Methods ")
* [Model Architecture](#model-architecture "Goto Model Architecture")
* [Hyperparameters](#hyperparameters "Goto Hyperparameters")
* [Results](#results "Goto Results")
## Description
In this project I have used autoencoder to train the network to colorise the grayscale images.
## Dataset
Dataset used for this project is torch.torchvision.datasets.Flowers102 which consists of RGB images of various types of flowers.
## Methods
* Autoencoder:I have used autoencoder in this project.Autoencoder is a neural network which is composed of encoder,bottleneck and a decoder.
 
* Transfer Learning: Transfer learning is the reuse of a pre-trained model on a new problem. In transfer learning, a machine exploits the knowledge gained from a previous task to improve   generalization about another.

* ResNet 18 Gray: Deep neural networks are hard to train as their depth increases. This increase in depth comes with many problems such as vanishing and exploding gradient descent . Residual Networks or ResNets are a solution to such problems.
In this project I have used Resnet 18 Gray which is a pretrained Convolutional neural network that is 18 layers deep,but I have used just first 6 layers of this    network.

* LAB Color Space: I have used LAB Color Space in this project as by separating out the lightness component, the neural network only has to learn the remaining two channels for colorization.

## Model Architecture
![Arcitecture](https://cdn.discordapp.com/attachments/993239385891942421/1030118698071101500/unknown.png)
## Hyperparameters 
|Hyperparameter |Description|
|-----|--------|
| Optimiser|Adam Optimiser      |
|Learning rate  | 0.001      |
| Loss Function | MSE loss |
| Batch size | 60 |

## Results
![Screenshot_116](https://user-images.githubusercontent.com/107758088/198269064-d19df0d2-4fcc-4471-bce1-44d4dfa23b7a.png)
![Screenshot_115](https://user-images.githubusercontent.com/107758088/198269117-8c5b166e-a90e-43a4-beaa-bc4e8aba973b.png)

![result2](https://user-images.githubusercontent.com/107758088/198271032-39c9253f-9b55-42b0-aa94-904b19c4e622.png)
![unknown2](https://user-images.githubusercontent.com/107758088/198271333-aa99bc7c-37df-40f4-ada5-3b4156cd4e4d.png)
