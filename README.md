Learning Probability Density Functions using GAN
Dataset

India Air Quality Dataset
Feature Used: NO2 concentration
## Dataset

The dataset used is the India Air Quality Dataset from Kaggle:

https://www.kaggle.com/datasets/shrutibhargava94/india-air-quality-data

Due to GitHub file size limitations, the dataset is not uploaded here.
Please download it from the above link and place `data.csv` in the project directory before running the notebook.

Transformation

z = x + a_r sin(b_r x)

Roll Number: 102316119
a_r = 1.5
b_r = 1.5

GAN Architecture
Generator

Input: 5D Gaussian noise

Two hidden layers (32 neurons each)

ReLU activations

Output: 1D sample

Discriminator

Input: 1D z value

Two hidden layers

Sigmoid output

Binary classification (real vs fake)

PDF Estimation

After training the GAN:

10,000 samples were generated

Kernel Density Estimation (KDE) used to estimate PDF

Histogram + KDE curve plotted

