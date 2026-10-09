<div align="center">

# 🐱🐶 Transfer Learning with VGG16

**Re-use a pre-trained VGG16 network to classify cat and dog photos with a small dense head on top.**

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?logo=keras&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)

</div>

---

## ✨ Overview

`TransferLearning_1.ipynb`:

1. 📦 Loads **VGG16** with ImageNet weights (`include_top=False`, input 150 × 150 × 3).
2. 🖼️ Reads images from `PetImages/` (train) and `PetImagesTest/` (test) with `ImageDataGenerator` (rescale, binary labels).
3. ➕ Adds a small head: `Flatten → Dense(256, relu) → Dropout(0.5) → Dense(1, sigmoid)`.
4. 🏋️ Trains for 30 epochs and evaluates on the test generator.

## 🚀 Getting Started

```bash
git clone https://github.com/Arashomranpour/Transfer_learning.git
cd Transfer_learning
pip install tensorflow numpy jupyter
jupyter notebook TransferLearning_1.ipynb
```

Prepare the data as one sub-folder per class (for example the Microsoft *Cats vs Dogs* `PetImages` set):

```
PetImages/      Cat/  Dog/
PetImagesTest/  Cat/  Dog/
```

## 📁 Project Structure

```
.
└── TransferLearning_1.ipynb
```

## 🛠️ Tech Stack

`TensorFlow` · `Keras` · `VGG16 (ImageNet)`
