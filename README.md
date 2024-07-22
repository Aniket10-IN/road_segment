# Satellite Roadway Segmentation

### Overview

This project focuses on identifying roadways from satellite images using deep learning techniques. The model used is a U-Net, a type of convolutional neural network (CNN) designed specifically for image segmentation tasks. The dataset includes high-resolution RGB satellite images and corresponding masks indicating road pixels.

## Dataset
Structure
Training Data: 6226 RGB satellite images (1024x1024 pixels) with masks.
Validation Data: 1243 RGB satellite images.
Test Data: 1101 RGB satellite images (without masks).
Labels
Road Pixels: White (255)
Background Pixels: Black (0)
#### Note: The mask values might not be exactly 0 and 255. Masks are binarized at a threshold of 128.

### Preprocessing

Histogram Equalization: Enhance the contrast of the images.
Binarization: Convert mask values to binary (0 or 1).

### Model Architecture
The U-Net model used consists of an encoder-decoder structure:

Encoder: Extracts features using convolutional layers.
Decoder: Reconstructs the image while retaining the location information.

### Lets test it from test dataset
![Screenshot from 2024-07-22 09-46-31](https://github.com/user-attachments/assets/1a8d79db-930e-423f-b10e-e6700d2db090)

