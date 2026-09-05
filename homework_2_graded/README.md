# Homework 2 (Graded) — Autodiff Engine + Keras Model Zoo

Two-part assignment: build a minimal automatic-differentiation library from scratch, then use Keras to solve four distinct classification problem types, each on a different dataset.

## Part I — Custom Autodiff

[`MNIST_Autodiff.ipynb`](MNIST_Autodiff.ipynb) implements a small `Tensor`/`Op` autograd system from scratch (`AddOp`, `MulOp`, a `Sigmoid` layer, etc., with reverse-mode gradient tracking) and trains an MNIST classifier on top of it — no NumPy/PyTorch autograd, no Keras, for the model itself.

## Part II — Four Keras Problem Types

| Notebook | Problem type | Dataset |
|---|---|---|
| [`keras_boolean_crossentropy.ipynb`](keras_boolean_crossentropy.ipynb) | Binary crossentropy | UCI Wine Quality (red vs. white) |
| [`Keras_categorical_crossentropy.ipynb`](Keras_categorical_crossentropy.ipynb) | Sparse categorical crossentropy (softmax) | Fashion-MNIST |
| [`Keras_Logistic_Regression.ipynb`](Keras_Logistic_Regression.ipynb) | Logistic regression (single softmax layer) | MNIST |
| [`Multi_Label_Classification.ipynb`](Multi_Label_Classification.ipynb) | Multi-label classification | [NanoNets multi-label food dataset](https://github.com/NanoNets/multi-label-classification-sample-python) — 10 overlapping labels (healthy, junk, dessert, protein, etc.) |

Each Keras notebook covers dropout, regularization, and proper weight initialization per the assignment brief, and includes an "Open in Colab" badge pointing back to this repo.

## Run it

Colab is the easiest path (badges are embedded in each notebook); locally, install from [`requirements.txt`](requirements.txt) (`keras`/`tensorflow`, `scikit-learn`, `pandas`, `opencv-python` for the multi-label notebook's image loading).
