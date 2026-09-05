# Homework 1 (Graded) — MNIST From Scratch

A feed-forward MNIST digit classifier implemented with **plain NumPy** — no Keras/PyTorch layers for the model itself. Keras is used only for data augmentation. The goal was to reimplement the core mechanics of a neural network (forward pass, backprop, gradient descent) by hand.

## What's implemented

From the assignment checklist ([`instructions.txt`](instructions.txt)):

- Mini-batch gradient descent with a tuned batch size
- A learning-rate schedule (adaptive across epochs)
- Dropout, with rates tuned per layer
- Proper random weight initialization
- Image augmentation on the training set only (via Keras `ImageDataGenerator`)
- 3+ fully-connected layers with ReLU activations
- Input normalization/scaling
- Training/testing accuracy curves, confusion matrix, and a breakdown of the most common misclassifications

## Notebook

[`MNIST_Rec_From_Scratch.ipynb`](MNIST_Rec_From_Scratch.ipynb) — structured as: load data → augment → normalize → one-hot encode labels → hand-written training loop (ReLU forward pass + mini-batch gradient descent) → training/test metrics.

## Run it

Open in Jupyter or Colab; dependencies are listed in [`requirements.txt`](requirements.txt) (NumPy, Keras/TensorFlow for `ImageDataGenerator` and the MNIST loader, matplotlib).
