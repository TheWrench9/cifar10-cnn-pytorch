# CIFAR-10 CNN Image Classification

A PyTorch-based CNN image classification project using the CIFAR-10 dataset.

## Features

- CIFAR-10 image classification
- Two-convolutional-layer CNN architecture
- Data augmentation with random cropping and horizontal flipping
- CIFAR-10 normalization
- 45,000 training images and 5,000 validation images
- Adam optimizer with weight decay
- Cosine learning-rate scheduling
- Training and validation loss/accuracy monitoring
- Best-model checkpointing
- Test-set evaluation
- Sample image inference
- Training performance visualization

## Model Architecture

```text
Input: 3 × 32 × 32

Conv2D: 3 → 32
BatchNorm
ReLU
MaxPool

Conv2D: 32 → 64
BatchNorm
ReLU
MaxPool

Flatten: 64 × 8 × 8 = 4096

Linear: 4096 → 256
ReLU
Dropout: 0.3

Linear: 256 → 10
