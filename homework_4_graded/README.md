# Homework 4 (Graded) — Classic CNN Architectures

Implements a set of well-known CNN architectures twice each — once in Keras, once in PyTorch — plus a transfer learning exercise, to compare the two frameworks directly on the same models.

## Contents

| Architecture | Keras | PyTorch | Dataset |
|---|---|---|---|
| LeNet-5 | [`LeNet_5_Keras.ipynb`](LeNet_5_Keras.ipynb) | [`LeNet_5_Pytorch.ipynb`](LeNet_5_Pytorch.ipynb) | MNIST |
| VGG16 | [`VGG16_Keras.ipynb`](VGG16_Keras.ipynb) | [`VGG16_Pytorch.ipynb`](VGG16_Pytorch.ipynb) | CIFAR-10 |
| ResNet | [`ResNet_Keras.ipynb`](ResNet_Keras.ipynb) | [`ResNet_Pytorch.ipynb`](ResNet_Pytorch.ipynb)¹ | CIFAR-10 |
| Transfer Learning | [`Transfer_Learning.ipynb`](Transfer_Learning.ipynb)¹ (Keras, pretrained VGG16) | — | CIFAR-10 |

¹ `ResNet_Pytorch.ipynb` and `Transfer_Learning.ipynb` were empty stubs in the original coursework. Both were added later: a ResNet-18 implementation in the same style as `VGG16_Pytorch.ipynb`, and a fine-tuned-pretrained-VGG16 notebook for transfer learning. Written to run correctly but **not executed** in this environment (no `torch`/`tensorflow` installed here) — no training outputs or accuracy numbers.

## Notes

- `LeNet_5_Pytorch.ipynb` and `VGG16_Pytorch.ipynb` load MNIST from local CSVs under [`mnist/`](mnist) rather than `torchvision.datasets`.
- `VGG16_Pytorch.ipynb` uses a `progress_bar` helper from [`utils.py`](utils.py), adapted from [kuangliu/pytorch-cifar](https://github.com/kuangliu/pytorch-cifar).
- [`checkpoint/ckpt.pth`](checkpoint) is a saved PyTorch model checkpoint from one of the training runs.
- CIFAR-10 (for the VGG16/ResNet notebooks) is fetched via `keras.datasets.cifar10` / `torchvision.datasets.CIFAR10` at runtime, not checked into the repo.

## Run it

Install from [`requirements.txt`](requirements.txt). Keras notebooks need `keras`/`tensorflow`; PyTorch notebooks need `torch`, `torchvision`, and (for `VGG16_Pytorch.ipynb`) a CUDA-capable GPU is assumed (`torch.device("cuda")` is hardcoded) — `ResNet_Pytorch.ipynb` auto-detects CUDA availability instead.
