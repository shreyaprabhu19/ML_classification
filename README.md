# MinorProject_DS23

This repository contains the codes for **Classification of astronomical X-ray transients using Machine Learning algorithm**. This project was supervised Dr. Shabnam Iyyani, Indian Institute of Science Education and Research (IISER) Thiruvananthapuram.

The Fermi Gamma-ray Burst Monitor (GBM) is an all-sky gamma-ray monitor that detects different types of hard X-ray transients such as gamma ray burst (GRB), terrestrial gamma ray flashes (TGF), solar flares (SF), short gamma ray repeaters (SGR) etc. The light curves of each class of triggers show different features which can be used to identify the trigger type. This project aims to develop an algorithm based on supervised machine learning technique to classify different types of transient triggers using their light curves which are time series data. In this direction, the current algorithm developed in the project is trained for identifying GRBs and TGFs using the convolutional neural network for the supervised clasification.

## Data
The data files are obtained from the Fermi GBM Trigger Catalog. The data files used in this project include a trigger data file (.fit extension) used to find the brightest detector and a Time-Tagged Event (TTE) data file used to plot the light curves.

## Algorithm for classification
A simple neural network model consisting of a single convolution layer gives the desirable accuracy on the training data set and can make predictions for unseen data with considerably high accuracy.
