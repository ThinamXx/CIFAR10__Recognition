# **CIFAR10: OBJECT RECOGNITION ON IMAGES**

**OBJECT RECOGNITION:**
- Object Recognition is a computer technology related to computer vision and image processing that deals with detecting instances of semantic objects of a certain class in digital images and videos. It has applications in many areas of computer vision, including image retrieval and video surveillance.

**LIBRARIS AND DEPENDENCIES:**
- I have listed all the necessary libraries and dependencies required for this project here:

```javascript
import os, collections, math
import shutil
import pandas as pd

import torch
import torchvision
from torch import nn
from d2l import torch as d2l
```

**OBTAINING AND ORGANIZING THE DATASET:**
- I have used google colab for this project so the process of downloading and reading the data might be different in other platforms. I will use [CIFAR-10 Object Recognition in Images](https://www.kaggle.com/c/cifar-10) for this project. The dataset is divided into training set and test set. The training set contains 50,000 images. The images contains the categories such as planes, cars, birds, cats, deer, dogs, frogs, horses, boats and trucks. I will organize the datasets to facilitate model training and testing. I have presented the implementation of Obtaining and Organizing the CIFAR10 Dataset here in the Snapshot.

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20157.PNG)

**IMAGE AUGMENTATION:**
- I will use image augmentation to cope with overfitting. The images are flipped at random and normalized. I have presented the implementation of Obtaining and Organizing the Dataset, Image Augmentation and Normalization using PyTorch here in the Snapshot. 

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20158.PNG)

**DEFINING THE MODEL:**
- I will define ResNet18 model. I will perform xavier random initialization on the model before training begins. I will define model training function train here. I will record the training time of each epoch which helps to compare costs of different models. I have presented the implementation Defining a Training Function using PyTorch here in the Snapshot. 

![Image](https://github.com/ThinamXx/300Days__MachineLearningDeepLearning/blob/main/Images/Day%20159.PNG)
