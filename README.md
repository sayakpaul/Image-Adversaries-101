# Adversarial Examples in Deep Learning

Deep Learning has brought us tremendous achievements in the field of Computer Vision. In spite of the impeccable success, modern Deep Learning systems are still prone to adversaries. Let's talk in terms of Computer Vision. Consider an image of a polar bear and an instance of it (X1). A Deep Learning-based image classifier is able to successfully X1 as a polar bear. Now consider another instance of a polar bear X2 which is a slightly perturbed version of X1. To the human eyes, it would still be a polar bear but for that same image classifier, it would be an ant. These perturbations are referred to as image adversaries.

<div align="center"><img src="https://i.ibb.co/Wkg8CSX/download.png"></img></div>

This repository contains code for a short crash-course related adversarial examples in deep learning. The crash course would include introduction to adversarial examples, training models that are adversarial-aware, situations where adversarial-aware models could fail, and so on.   

The crash course would be presented in form of [Weights and Biases reports](https://docs.wandb.com/reports). The first report in this line is now up - 
- [An Introduction to Adversarial Examples in Deep Learning](https://app.wandb.ai/authors/adv-dl/reports/An-Introduction-to-Adversarial-Examples-in-Deep-Learning--VmlldzoyMTQwODM)

## Contents (to be updated):
- `Image_Adversaries_Basics.ipynb`: Shows how to create adversaries that can fool a ResNet50 model pre-trained on ImageNet. Includes both vanilla and targeted attacks. 
- `Adversarial_Training_NSL.ipynb`: Shows how to train adversarially robust image classifiers using [`Neural Structured Learning`](https://www.tensorflow.org/neural_structured_learning). 
- `GANs_w_Adversaries.ipynb`: Shows how to incorporate GANs (plain old DCGAN) to tackle adversarial situations. 
- `Optimizer_Susceptibility.ipynb`: Studies the susceptibility of different optimizers against simple attacks.
- `Optimizer_Susceptibility_Targeted_Attacks.ipynb`: Studies the susceptibility of different optimizers against targeted attacks.

**Note**: The materials are strictly for learning purpose and should not be considered for production systems.

## Coded in:
- TensorFlow 2.x (at time of writing Google Colab had TensorFlow `2.3.0`)

## References:
- [J. Z. Kolter and A. Madry: Adversarial Robustness - Theory and Practice (NeurIPS 2018 Tutorial)](https://adversarial-ml-tutorial.org/)
- Chapter 10 (Adversarial examples), [GANs in Action](https://www.manning.com/books/gans-in-action)
- [Introduction to Adversarial Machine Learning](https://blog.floydhub.com/introduction-to-adversarial-machine-learning/)
- [Adversarial example using FGSM](https://www.tensorflow.org/tutorials/generative/adversarial_fgsm)
- [Adversarial regularization for image classification](https://www.tensorflow.org/neural_structured_learning/tutorials/adversarial_keras_cnn_mnist)
