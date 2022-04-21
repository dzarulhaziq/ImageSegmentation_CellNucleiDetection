# Cell Neuclei Detection using Semantic Segmentation with U-Net

## 1. Summary
- The aim of the project is to detect cell nuclei from biomedical images effectively.
- The cell nuclei vary in shapes and sizes, semantic segmentation proves to be the best approach to detect them. 
- A deep learning model is trained and deployed for this task. The model is trained with the well known [2018 Data Science Bowl dataset.](https://www.kaggle.com/c/data-science-bowl-2018)

## 2. IDE and Framerowk

- The project is built with Spyder as the main IDE.
- The main frameworks used in this project are :
~~~bash
import numpy as np
import pandas as pd 
import matplotlib.pyplot as plt
import glob
import pathlib
import tensorflow as tf
from tensorflow import keras
import os
from tqdm import tqdm
import time
import datetime
~~~

## 3. Methodology
- The methodology is inspired by a documentation available in the official TensorFlow website. You can refer to the documentation here.
### 3.1 Input Pipeline

In the format of images for inputs and image masks for labels, the dataset files contain a train folder for training data and a test folder for testing data in the format of images for inputs and image masks for labels. Feature scaling is used to preprocess the input photos. The labels have been preprocessed to have binary values of 0 and 1. The dataset does not have any data augmentation. The train data is divided into train-validation sets in an 80:20 ratio.

### 3.2 Model Pipeline

The model architecture used for this project is U-Net. You can refer to the TensorFlow documentation for further details. In summary, the model consist of two components, the downward stack, which serves as the feature extractor, and upward stack, which helps to produce pixel-wise output. The model structure is shown in the figure below.

![20220421-202106_train (1)](https://user-images.githubusercontent.com/103733709/164468583-af36c696-2259-4952-b043-18edccdf7ef9.png)
