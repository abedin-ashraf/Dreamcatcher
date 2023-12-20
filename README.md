# DCGAN-CS505: Unsupervised Generative Adversarial Networks using Deep Convolutional Networks

## Project Overview

This repository contains the implementation and findings of a group project conducted during the Fall 2023 semester as part of the CS505-01 Data Mining course at Southeast Missouri State University. The project focuses on exploring the application of Deep Convolutional Generative Adversarial Networks (DCGANs) for unsupervised learning.

## Group Members

- Mohammed Nurul Abedin Ashraf
- Sheshanth Reddy Ananthula
- Krishna Sai Bezavada
- Saikrishna Karnati
- Sindhu Mandalapu

## Abstract

This project addresses the gap between the success of Convolutional Neural Networks (CNNs) in supervised learning and their underutilization in unsupervised learning. By introducing Deep Convolutional Generative Adversarial Networks (DCGANs), a subclass of CNNs with specific architectural restrictions, we aim to demonstrate their promise for unsupervised learning. The hierarchical representation learning of objects and scenes by both the generator and discriminator is explored, showcasing the effectiveness of DCGANs as general image representations.

## 1. Introduction

The project focuses on learning reusable feature representations from large unlabeled datasets using generative adversarial networks (GANs). The key contributions include:

- Introducing stable-to-train Convolutional GANs, referred to as Deep Convolutional GANs (DCGAN).
- Utilizing trained discriminators for image classification tasks, surpassing previous unsupervised algorithms.
- Empirically demonstrating how filters have learned to draw objects and the intriguing vector arithmetic properties of generators.

## 2. Related Works

The project discusses representation learning from unlabeled data, generative models for natural images, and techniques for visualizing the internals of Convolutional Neural Networks (CNNs).

## 3. Approach and Model Architecture

The project outlines the architectural modifications made to scale up GANs using CNNs, including the use of strided convolutions, removal of fully connected layers, and the application of batch normalization. The model architecture adheres to specific guidelines, such as using Tanh activation in the output layer and LeakyReLU activation in the discriminator.

## 4. Details of Adversarial Training

The training details include the use of datasets such as LSUN, Imagenet-1k, and a Faces dataset. The implementation employs a mini-batch size of 32, normal distribution for weights, and the Adam optimizer with customized hyperparameters. The LSUN scenario is used as an example to illustrate the DCGAN generator.

### 4.1 Adding Convolutional Layers to GANs

The project introduces the primary idea of DCGANs, emphasizing the addition of up-sampling convolutional layers and the removal of fully connected layers. It discusses concepts such as batch normalization, leaky ReLU activation, and the LSUN dataset.

## 5. Conclusions

The conclusions highlight the stability of the proposed topologies for training generative adversarial networks. The project demonstrates that these networks can learn accurate representations for both supervised learning and generative modeling. It also acknowledges limitations due to hardware and time constraints.

## 6. Future Work

Future work suggestions include implementing Progressive Growing GAN, monitoring metrics such as loss and accuracy, visualizing the model graph, and projecting embeddings to a lower-dimensional space.

## Acknowledgments

The group expresses gratitude for the support and suggestions received throughout the project, including valuable input from Ian Goodfellow, Tobias Springenberg, Arthur Szlam, Durk Kingma, and the Indico research team. Special thanks to Nvidia for providing a Titan-X GPU for the project.

## References

The project refers to various works, including those by James Bergstra, Yoshua Bengio, Adam Coates, Andrew Ng, and Jia Deng, among others.
