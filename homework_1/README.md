# Homework 1 — fast.ai Lesson 1–2 Redo

## Assignment Brief

- Watch fast.ai *Practical Deep Learning for Coders* — Part 1, Lessons 1 and 2.
- Redo the lesson 1 and lesson 2 Colabs against a **different** dataset/problem than the course examples.
- Separately, read through the TensorFlow "classification" and "quickstart" tutorials and redo the Keras classification tutorial on another task.
- Work from scratch — no copy-pasting the reference Colabs.

See [`instructions.txt`](instructions.txt) for the original wording.

## Notebook

[`fastai_lesson1_2_redo.ipynb`](fastai_lesson1_2_redo.ipynb) — scene classification on the [Intel Image Classification dataset](https://www.kaggle.com/datasets/puneet6060/intel-image-classification) (buildings/forest/glacier/mountain/sea/street), using `fastai`'s `vision_learner` on a ResNet-34 backbone (lesson 1 style: transfer learning, `fine_tune`), then interpreting errors with a confusion matrix and top-losses, unfreezing, and fine-tuning further (lesson 2 style).

> **Note:** this notebook did not exist in the original 2020 coursework — only the assignment brief was ever committed. It was added later to close that gap. It's written to run correctly in a standard fastai/Colab environment, but hasn't been executed here (no `fastai`/`torch` installed in this environment), so there are no training outputs or accuracy numbers attached.

Distinct from [`homework_1_graded`](../homework_1_graded) — that's a separate, later graded assignment (a from-scratch NumPy MNIST classifier), not a resubmission of this one.

## Run it

Install from [`requirements.txt`](requirements.txt) (`fastai`, which pulls in `torch`/`torchvision`).
