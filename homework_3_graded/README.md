# Homework 3 (Graded) — Planet Amazon CNN Classification

A Keras CNN trained on the [Planet: Understanding the Amazon from Space](https://www.kaggle.com/c/planet-understanding-the-amazon-from-space) dataset, with TensorBoard instrumentation across multiple training runs.

## Notebook

[`Amazon_Data_Classification.ipynb`](Amazon_Data_Classification.ipynb) — loads the training/test imagery, builds and trains a CNN classifier (Keras, not PyTorch — required by the assignment), and iterates across several hyperparameter/architecture variations while logging to TensorBoard.

## TensorBoard

Six separate training runs' raw event logs are checked in under [`logs/`](logs) (one `train/` + `validation/` pair per run, timestamped `20200511-*`). A snapshot of the TensorBoard UI is saved as [`tensorboard.JPG`](tensorboard.JPG).

To view them locally:

```bash
tensorboard --logdir logs
```

**Gap:** the assignment asked for the results to also be published to [tensorboard.dev](https://tensorboard.dev) for easy sharing — only the local event logs survive in this repo; no hosted link was committed.

## Run it

Install from [`requirements.txt`](requirements.txt) (`keras`/`tensorflow`, TensorBoard). The notebook downloads/reads the Planet Amazon dataset directly — not included in this repo due to size.
