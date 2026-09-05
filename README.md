# Deep Learning — Coursework & Experiments

Archive of lab work, assignments, and a literature survey from a graduate-level **Deep Learning** course (CMPE 258, San José State University, Spring 2020). Everything here was built from scratch as coursework — plain NumPy implementations early on, moving to Keras/TensorFlow and PyTorch as the term progressed.

Author: Manmeet Singh

## Repository Map

| Folder | Topic | Stack |
|---|---|---|
| [`homework_0`](homework_0) | Warm-up: NumPy broadcasting, Jupyter/Markdown basics, math refresher, an end-to-end regression project | NumPy, pandas, scikit-learn |
| [`homework_1`](homework_1) | fast.ai lesson 1–2 redo (scene classification) | fastai |
| [`homework_1_graded`](homework_1_graded) | MNIST digit classifier written from scratch with NumPy | NumPy |
| [`homework_2_graded`](homework_2_graded) | Custom autodiff engine + four Keras model types (binary/categorical crossentropy, logistic regression, multi-label classification) | Keras, TensorFlow |
| [`homework_3_graded`](homework_3_graded) | Multi-label CNN on the Planet: Amazon rainforest dataset, with TensorBoard instrumentation | Keras, TensorBoard |
| [`homework_4_graded`](homework_4_graded) | Classic CNN architectures (LeNet-5, VGG16, ResNet) and transfer learning, implemented in both Keras and PyTorch | Keras, PyTorch |
| [`FaceDataAugmentationSurvey`](FaceDataAugmentationSurvey) | Literature survey and presentation on GAN-based face data augmentation | — |

Each folder has its own README with assignment context, what was implemented, and how to run it. Each folder also has a `requirements.txt` listing the packages its notebooks import.

## Environment

Notebooks target Python 3 with `numpy`, `pandas`, `matplotlib`, `scikit-learn`, `keras`/`tensorflow`, and `torch`/`torchvision`. Most were originally authored and executed in Google Colab, and several retain their "Open in Colab" badges. Per-folder `requirements.txt` files list what each assignment imports, inferred from the notebooks rather than pinned at the time — see [Known Gaps](#known-gaps) for the version-drift caveat that comes with that.

## Known Gaps

Revisiting this repository years later surfaced a few loose ends. Some were fixed directly; others can't honestly be fixed after the fact and are documented instead:

**Fixed:**

- **`homework_0/g_math_practice.ipynb`** was an empty notebook — added a linear algebra/calculus refresher (vectors, gradients, chain rule, gradient descent, softmax) matching the spirit of the other warm-up exercises.
- **`homework_1/`** previously held only the assignment brief with no submitted notebook. Added [`fastai_lesson1_2_redo.ipynb`](homework_1/fastai_lesson1_2_redo.ipynb), redoing fast.ai lessons 1–2 on an Intel scene-classification dataset.
- **`homework_4_graded/ResNet_Pytorch.ipynb`** and **`homework_4_graded/Transfer_Learning.ipynb`** were empty stubs — added a ResNet-18/CIFAR-10 implementation and a pretrained-VGG16 fine-tuning notebook, respectively.
- **No `requirements.txt`** existed for any assignment — added one per folder, generated from each notebook's actual imports.

  ⚠️ All four backfilled notebooks above were written to satisfy their assignment briefs and are believed correct, but this environment has no `torch`/`tensorflow`/`fastai` installed, so **none of them have actually been executed** — no training was run and no accuracy numbers were produced. They're a later addition, not part of the original 2020 submissions; each carries a note to that effect in its own README/notebook header.

**Left as documented gaps** (not something a repo cleanup can retroactively fix, or requires action outside this repo):

- **No dependency/version pinning** — several original notebooks use APIs (`keras.datasets`, standalone `keras` rather than `tf.keras`, older `torchvision` transforms) reflecting 2020-era library versions that may not run unmodified on current releases.
- **Large binary artifacts committed directly to git**: `homework_4_graded/mnist/{train,test}.csv` (~123 MB combined), `homework_4_graded/checkpoint/ckpt.pth` (57 MB), and `FaceDataAugmentationSurvey/Presentation_video.mp4` (14 MB). Moving these to Git LFS would require rewriting history and force-pushing to the live `origin` remote — left untouched pending an explicit decision to do that.
- **`homework_3_graded`**'s assignment required publishing results to tensorboard.dev; only the raw local TensorBoard event logs were committed. Publishing now would put 6-year-old logs on a public hosted service under a personal account, so it was left undone rather than done silently.

## License

Coursework and personal project archive, shared as-is for reference. No license is granted for reuse of the associated course materials (assignment briefs, linked datasets).
