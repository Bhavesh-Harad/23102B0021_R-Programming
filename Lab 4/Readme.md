# Lab 4: Image Classification using Deep Learning in R

## Project Overview
This repository contains the R programming implementation for Lab 4, which demonstrates how to build a basic image classification model using deep learning[cite: 5]. Utilizing the `keras3` and `jpeg` packages, this lab implements a fully connected Artificial Neural Network (ANN) to classify images into two distinct categories: **Planes (Class 0)** and **Cars (Class 1)**[cite: 5].

## Key Tasks Implemented
The R script systematically executes the following deep learning pipeline:
*   **Image Import & Preprocessing:** Reads JPEG images and passes them through a custom `resize_image()` function to standardize all inputs to 28x28 pixels across 3 color channels (RGB)[cite: 5].
*   **Data Flattening:** Reshapes the 3D image arrays into 1D feature vectors containing 2,352 pixels each to feed into the dense neural network[cite: 5].
*   **Data Splitting & Encoding:** Separates the images into a training set and a testing set, maps the labels (0 for planes, 1 for cars), and applies one-hot encoding (`to_categorical`) for the output layer[cite: 5].
*   **Model Architecture:** Constructs a sequential neural network consisting of:
    *   Input/Hidden Layer 1: 256 units with ReLU activation[cite: 5].
    *   Hidden Layer 2: 128 units with ReLU activation[cite: 5].
    *   Output Layer: 2 units with Softmax activation for binary probability distribution[cite: 5].
*   **Compilation & Training:** Compiles the model using the `rmsprop` optimizer and `categorical_crossentropy` loss function, then trains it for 30 epochs with a 20% validation split[cite: 5].
*   **Evaluation & Prediction:** Evaluates the model's accuracy on the dataset and generates a comparison matrix mapping the predicted classes against the actual ground-truth labels[cite: 5].

## Repository Files
*   **`p1.jpg` to `p6.jpg`:** The image dataset representing the "Planes" class[cite: 5].
*   **`c1.jpg` to `c6.jpg`:** The image dataset representing the "Cars" class[cite: 5].
*   **`results.png`:** A console output snapshot displaying the model's predicted probabilities alongside a table comparing the Predicted vs. Actual values[cite: 5].
*   **`Lab4.R`** *(or your specific filename)*: The main R script containing the Keras neural network pipeline[cite: 5].
