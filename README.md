# Classification of Astronomical X-ray Transients Using Machine Learning Algorithm
## Data Science Minor Project 2023

This repository contains the codes for **Classification of astronomical X-ray transients using Machine Learning algorithm**. This project was supervised Dr. Shabnam Iyyani, Indian Institute of Science Education and Research (IISER) Thiruvananthapuram.

The Fermi Gamma-ray Burst Monitor (GBM) is an all-sky gamma-ray monitor that detects different types of hard X-ray transients such as gamma ray burst (GRB), terrestrial gamma ray flashes (TGF), solar flares (SF), short gamma ray repeaters (SGR) etc. The light curves of each class of triggers show different features which can be used to identify the trigger type. This project aims to develop an algorithm based on supervised machine learning technique to classify different types of transient triggers using their light curves which are time series data. In this direction, the current algorithm developed in the project is trained for identifying GRBs and TGFs using the convolutional neural network for the supervised clasification.

## Data
The data files are obtained from the Fermi GBM Trigger Catalog. The data files used in this project include a trigger data file (.fit extension) used to find the brightest detector and a Time-Tagged Event (TTE) data file used to plot the light curves.

## Light Curves of Different X-ray Transients
Light curves are graphs that show the brightness of an object in terms of number of photons as a function of time. Light curves for different triggers are obtained by plotting histograms of the time data present in the TTE file. The features visible in these light curves vary depending on the trigger type. A few light curves for random triggers were plotted to visualize these features.

![Light_curves1](https://github.com/user-attachments/assets/a03d71ba-37be-4468-888b-e067d02cd919)

Light curves for Gamma Ray Burst (GRB) and terrestrial gamma ray flash (TGF) for different bin sizes are shown in the following figure.

![Screenshot (5)](https://github.com/user-attachments/assets/f62cb87f-e2bb-4ba0-b451-6fc53f0bf451)

## Algorithm for Classification
A simple neural network model consisting of a single convolution layer gives the desirable accuracy on the training data set and can make predictions for unseen data with considerably high accuracy.

The code <code>Classification_using_CNN.ipynb</code> consists of the supervised classification algorithm using the Convolotional Neural Network. The early stopping techniques is also implemented to prevent the model from overfitting. The model for classifying the two classes of transients (GRBs and TGFs) work with the accuracy of 68% for the considered testing data.
