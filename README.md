# My Project
# Threat Detection in Videos using Faster R-CNN 🎥🚨

## Overview

This repository provides a Threat Detection solution using the Faster R-CNN (Region-based Convolutional Neural Network) model for analyzing videos. The model is trained to detect threats within video frames, making it a valuable tool for security and surveillance applications.

## 📋 Table of Contents

1. [Introduction](#introduction)
2. [Setup](#setup)
3. [Training](#training)
4. [Testing](#testing)
5. [Validation](#validation)
6. [Usage](#usage)
7. [Contributing](#contributing)
8. [License](#license)

## 🚀 Introduction

The Faster R-CNN model is employed to identify threats within video frames. This solution allows for efficient threat detection and is customizable based on your dataset.

## ⚙️ Setup

To get started, follow these steps:

- Clone this repository to your local machine.
- Install the required dependencies by running `pip install -r requirements.txt`.
- Ensure that your dataset is organized with CSV annotations and image directories.

## 🚂 Training

To train the model, use the following command:

```bash
python train.py -cp <path_to_csv> -ip <path_to_images> -mp <main_directory_path> -simg <sample_image_count> -e <epochs> -sm <save_model_flag>
```

- `-cp` or `--csv_path`: Path to the CSV file containing annotations.
- `-ip` or `--image_path`: Path to the directory containing images.
- `-mp` or `--main_directory_path`: Path to the main directory.
- `-simg` or `--sample_image`: Number of total data samples.
- `-e` or `--epochs`: Number of training epochs.
- `-sm` or `--save_model`: Specify True if you want to save the trained model.

## 🧪 Testing

To test the model, use the following command:

```bash
python test.py -fp <file_path_to_test_image> --test_model True
```

- `-fp` or `--file_path`: Path to the image for testing.
- `--test_model`: Specify True to enable testing mode.

## ✔️ Validation

Validation is an integral part of the training process, ensuring the model's generalization. During training, a portion of the dataset is used for validation. Adjust the parameters accordingly to achieve optimal performance.

## 🛠️ Usage:

[![Watch the video](https://github.com/shiv2398/Threat_detection_using-Deep_learning/blob/main/How%20to%20defend%20against%20a%20knife%20attack.gif)
