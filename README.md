# Deep Learning Assignment - Caltech-256 Classification

## Overview

This project implements a Convolutional Neural Network (CNN) for image classification using the Caltech-256 dataset. The model is trained using different optimizers and hyperparameters to achieve optimal performance.

## Dataset Details:

- **Dataset Used:** Caltech-256
- **Number of Classes:** 256 object categories
- **Training Set:** 70% of images
- **Validation Set:** 15% of images
- **Test Set:** 15% of images
- **Image Size:** 128 × 128 pixels (resized)

## Model Implementation:

- **Model Type:** Convolutional Neural Network (CNN)
- **Hidden Layers:** Configurable (Conv2D, MaxPooling, Fully Connected Layers)
- **Activation Functions:** ReLU
- **Optimizers Tested:** SGD, Adam, RMSprop, Momentum-based SGD, Nesterov Accelerated Gradient Descent
- **Loss Functions:** Cross-Entropy Loss and Mean Squared Error (MSE)
- **Batch Sizes Tested:** 16, 32, 64
- **Learning Rates:** 0.001, 0.0005
- **Weight Initialization:** Random, Xavier

## Training and Evaluation:

- The model is trained for multiple epochs using different configurations.
- Training and validation losses were monitored for model performance.
- Cross-Entropy Loss and Mean Squared Error Loss were compared.
- A confusion matrix was generated to visualize classification performance.

## Results and Best Model Selection:

The model was trained with different hyperparameter settings, and the accuracy results are as follows:

- **For a CNN with 3 Conv layers using Adam optimizer (LR=0.001, Batch Size=32), test accuracy was 78.12%.**
- **For a CNN with 4 Conv layers using SGD optimizer (LR=0.0005, Batch Size=64), test accuracy was 72.43%.**
- **For a CNN with 2 Conv layers using RMSprop optimizer (LR=0.001, Batch Size=16), test accuracy was 69.85%.**

**Best Configuration Selected:**

- **Architecture:** CNN with 3 Conv Layers
- **Optimizer:** Adam
- **Batch Size:** 32
- **Learning Rate:** 0.001

## Loss Function Comparison:

A comparison between Cross-Entropy Loss and Mean Squared Error (MSE) Loss showed:

- **Cross-Entropy Loss:** 0.8921
- **Mean Squared Error (MSE) Loss:** 5.4312

Cross-Entropy Loss significantly outperformed MSE Loss, confirming that it is more suitable for multi-class classification tasks.

## How to Run the Code:

### Clone the repository:

```sh
git clone https://github.com/Udvik/DL_ASSIGNMENT_1
cd <repo-folder>
```

### Run the project:

1. Open `caltech256_classification.ipynb` in Google Colab or Jupyter Notebook.
2. Run all the cells in order.
3. Check the model accuracy, loss values, and confusion matrix at the end.

##

