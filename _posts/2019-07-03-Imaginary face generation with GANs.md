---
title: "Imaginary face generation with GANs"
header:
  overlay_image: /assets/images/udacity5.jpg
  caption: "Photo credit: [**h heyerlein**](https://unsplash.com/@heyerlein)"
  cta_url: "https://github.com/dcarlyle/udacity_deep_learning_foundations__P_5/blob/master/dlnd_face_generation.ipynb"
categories:
  - Machine learning
  - Development
  - Udacity
  - Education
  - Neural network
tags:
  - python
  - coding
  - GAN
last_modified_at: 2019-07-03T11:45:09-04:00
---

# Face generation

![alt text](https://raw.githubusercontent.com/dcarlyle/udacity_deep_learning_foundations__P_5/master/wireframe_face_udacity.png "Face wireframe") In this project I developed a Generative adversarial network (GAN) to create photo-realistic images of people. The machine learning algorithm didn't simply look up images of faces from a database, each image was generated at random by the algorithm and is totally imaginary.

GANs use two neural networks, one to generate the image and the adversary to distinguish between the real item and the forgery. In essence they work like a *criminal forging money* and a *policeman* whose job it is to find the forgeries. Over a period of time the policeman becomes better at detecting fake money, so the criminal has to learn to improve the quality of the forgery.

## The results
Just after a few hours of training we can see the output starting to produce quite realistic images of human faces.

![alt text](https://raw.githubusercontent.com/dcarlyle/udacity_deep_learning_foundations__P_5/master/generated_faces.png "Face creation with GANs")


## Training the GAN
The GAN was initially trained on the simple [MINST handwritten database](https://en.wikipedia.org/wiki/MNIST_database), to quickly check the design, performance and accuracy of the convolutional neural networks (CNN) that is used to deconstruct and recreate images. 

Using a simpler data set to test the structure and output of the two machine learning AI algorithms was a quick and cheaper way to iron out any early issues with the structures.


## Platform and tools
The neural networks were programmed in Python using Jupyter notebook. 

The code was deployed to a Linux AWS server instance using multiple GPU (Graphic processing units). The Nvidia GPUs are particularly good at matrix and tensor (multi-dimensional or cubes) arithmetic (certainly a lot better than my MAC's CPU and AMD chips).


## A bit more about GANs
According to [Yann LeCun](https://medium.com/@devnag/generative-adversarial-networks-gans-in-50-lines-of-code-pytorch-e81b79659e3f)(director of Facebook AI) "General Adversarial Networks is the most **interesting idea in the past ten years** in machine learning."

In 2014 Ian Goodfellow returned home from a going away drinks at the bar, where he and his friends were discussing issues around the inefficient method by which a machine learning algorithm learns about unlabelled data. For example a child learns to recognise a letter in the alphabet that their teacher shows them, they only need to see it a few times, where as a machine learning algorithm needs to be shown thousands of variations of the same letter before they can perform the same image recognition task.

That night Ian went home and coded up a simple prototype of the GAN to learn to recognise the numbers in the MINST data set. It worked and led to the [following paper](https://arxiv.org/pdf/1406.2661.pdf) being released to [NIPS (Neural Information Processing Systems)](https://nips.cc/About)

## Code
* [code archive](https://github.com/dcarlyle/udacity_deep_learning_foundations__P_5)
* [jupyter notebook](https://github.com/dcarlyle/udacity_deep_learning_foundations__P_5/blob/master/dlnd_face_generation.ipynb)

## Review
[Code review](https://github.com/dcarlyle/udacity_deep_learning_foundations__P_5 "Code reivew")
