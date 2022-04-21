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
~~~

## 3.

![20220421-202106_train (1)](https://user-images.githubusercontent.com/103733709/164468583-af36c696-2259-4952-b043-18edccdf7ef9.png)
