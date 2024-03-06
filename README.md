# Traffic Sign Recognition (TSR) System using Convolutional Neural Networks (CNN)

## Project Overview

This project aims to develop a Traffic Sign Recognition (TSR) system using Convolutional Neural Networks (CNN). The system is designed to classify a wide range of traffic road signs in Singapore, including directional signs, warning signs, and regulatory signs. The objective is to facilitate the safe navigation of autonomous vehicles by accurately detecting and classifying road signs.

## Business Requirements

The primary business requirement is to classify two specific traffic signs: the "U-turn" sign and the "Stop" sign. These signs are crucial for ensuring the safety and efficiency of autonomous vehicles on the road.

## Dataset Collection

- Images of the "U-turn" and "Stop" signs were collected from various sources, including the Land Transport Authority of Singapore (LTA) website.
- The images were cropped and stored in the `data` folder within their respective subfolders (`U-turn` and `Stop`).

## Data Preprocessing

- The images were resized to a standard size of 100x100 pixels.
- Data augmentation techniques, including brightness adjustment, rotation, horizontal and vertical shifts, and zoom, were applied to enhance the diversity of the dataset.

## Model Architecture

- The CNN model consists of two convolutional layers followed by max-pooling operations, a flattening layer, dropout regularization, and fully connected layers.
- The model uses the Adam optimizer with a learning rate of 0.001 and employs the sparse categorical cross-entropy loss function.
- The training was conducted using GPU acceleration to expedite the process.

## Training and Evaluation

- The dataset was split into training and test sets using a random seed of 42.
- The model was trained for 10 epochs, with a batch size of 32.
- Model checkpoints were saved during training to preserve the model's state.
- The model achieved a test accuracy of 1.0 and a perfect F1 score, indicating excellent performance.

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your_username/traffic-sign-recognition.git
