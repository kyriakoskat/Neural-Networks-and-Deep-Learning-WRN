# Neural Networks and Deep Learning – WRN Assignment

This repository contains code and experiments for an assignment in the Neural Networks and Deep Learning course. In this project, we implement and evaluate various Wide Residual Networks (WRNs) on CIFAR-10 and assess their generalization performance on CIFAR-C (a corrupted version of CIFAR-10). We also study the impact of mixup data augmentation on the robustness and confidence calibration of these models.

## Project Overview

Wide Residual Networks have been shown to achieve state-of-the-art performance with significantly fewer layers than traditional deep residual networks by increasing the width of the layers. In this assignment we:
- Experiment with different model configurations (varying depth, widening factor, and dropout) based on the paper ["Wide Residual Networks"](https://arxiv.org/abs/1605.07146) by Zagoruyko and Komodakis.
- Evaluate the effect of regularization via dropout.
- Continue training the best model further on CIFAR-10 and then apply mixup data augmentation. Mixup is used to enhance the generalization ability by creating virtual training examples through linear interpolations of data pairs.
- Evaluate the final models on CIFAR-C to measure robustness against various corruptions.
- (Bonus) Analyze the average confidence scores (softmax output on correct predictions) per class with and without mixup, and plot the results to understand the effects on model calibration.

### WideResNet Architecture (`widerstnet.py`)

This repository includes the file `widerstnet.py`, which contains the implementation of the Wide Residual Network (WRN) architecture used in our experiments. Please note that I did not originally develop this implementation. The code was adapted from the lab to serve as a baseline for this project. 


