# Detection-of-Pneumonia-from-X-Ray-Images-of-Lungs-Using-CNN
Classifying X-Ray images of lungs as "Normal" or "Pneumonia" affected from COVID-19 X-Ray images

# Data
Original dataset taken from https://www.kaggle.com/khoongweihao/covid19-xray-dataset-train-test-sets and Joseph Paul Cohen and Paul Morrison and Lan Dao. COVID-19 image data collection, arXiv, 2020. https://github.com/ieee8023/covid-chestxray-dataset

Train folder conatains:
  74 X-Ray images of normal lungs;
  74 X-Ray images of Pneumonia affected lungs.

Test folder conatains:
  20 X-Ray images of normal lungs;
  20 X-Ray images of Pneumonia affected lungs.

# Requirements
1) Python3
2) TensorFlow
3) Keras
4) matplotlib
5) os
6) logging

# Model
CNN with 5 convolutional layers, each followed by a max pooling layer (filter dim: 3 x 3, pooling dim: 2 x 2, stride = 1);

Loss function: binary crossentropy;

Optimiser: Adam with 0.001 learning rate;

Activation fucntion: reLU in all layers except for the last one which uses sigmoid;

# Pre- processing

Please rename "train_NORMAL" and "train_PNEUMONIA" to "NORMAL" and "PNEUMONIA" instead and put the two folders in a single forlder called "train"
