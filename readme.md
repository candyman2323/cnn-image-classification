# CNN Image Classification using MobileNetV2

A deep learning project for classifying images into six categories using a custom Convolutional Neural Network (CNN) and MobileNetV2 transfer learning with TensorFlow and Keras.

## Overview

Image classification is a computer vision task in which a model learns to assign an image to one of several predefined classes.

This project explores two approaches:

- **Custom CNN:** learns image features through convolutional and pooling layers.
- **MobileNetV2:** uses a pretrained convolutional neural network as a starting point for transfer learning.

The project uses a six-class image classification dataset organized into training and testing directories.

## Features

- Image classification across six categories.
- CNN-based image feature extraction.
- Transfer learning using MobileNetV2.
- Training and evaluation using TensorFlow and Keras.
- Comparison of a custom CNN approach with a pretrained model approach.

## Technologies Used

- Python
- TensorFlow
- Keras
- MobileNetV2
- NumPy
- Matplotlib
- Scikit-learn

## Dataset

The project uses the Intel image classification dataset with six categories:

- Buildings
- Forest
- Glacier
- Mountain
- Sea
- Street

Expected directory structure:

```text
seg_train/
└── seg_train/
    ├── buildings/
    ├── forest/
    ├── glacier/
    ├── mountain/
    ├── sea/
    └── street/

seg_test/
└── seg_test/
    ├── buildings/
    ├── forest/
    ├── glacier/
    ├── mountain/
    ├── sea/
    └── street/
```

Each class directory contains images belonging to that category. Keep the folder names consistent with the dataset and the class-loading logic in the code.

## Project Structure

```text
CNN-Image-Classification/
├── seg_train/
├── seg_test/
├── main.py
├── requirements.txt
└── README.md
```

## Installation

### 1. Install the dependencies

```bash
python -m pip install tensorflow numpy matplotlib scikit-learn
```

If a `requirements.txt` file is included, install the project's listed dependencies with:

```bash
python -m pip install -r requirements.txt
```

### 2. Prepare the dataset

Download and extract the image dataset. Place the training and testing folders in the locations expected by the code.

## Run the Project

Open a terminal in the project directory and run:

```bash
python main.py
```

The script should execute the model-training and evaluation workflow implemented in the project.

## Models

### Custom CNN

A CNN learns spatial features from images through convolutional operations and pooling layers. Its final classification layers map the learned features to the target classes.

### MobileNetV2 Transfer Learning

MobileNetV2 is a pretrained convolutional neural network that can provide useful image features. Transfer learning adapts the model for the six target classes by configuring the classification output for this dataset and training the selected layers as implemented in the project.

## Evaluation

The model's performance should be assessed using the evaluation procedures included in the code, such as classification accuracy or other classification metrics when implemented.

No specific accuracy result is stated here because it depends on the actual training run, dataset preparation, and model configuration.

## Learning Outcomes

- Understanding CNN architectures for image classification.
- Preparing image datasets for deep learning.
- Applying transfer learning with MobileNetV2.
- Training models using TensorFlow and Keras.
- Evaluating image classification models.

## Limitations

Performance depends on dataset quality, image preprocessing, training configuration, and the similarity between training images and images encountered during prediction.