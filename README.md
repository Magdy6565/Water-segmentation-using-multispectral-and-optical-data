# Water-segmentation-using-multispectral-and-optical-data

# Overview
This project uses a U-Net model for image segmentation tasks. The model is trained on a dataset of multi-channel TIFF images and corresponding binary masks. Data augmentation techniques are employed to enhance the dataset and improve model performance.



# Requirements
Ensure you have the following Python packages installed:

TensorFlow (2.x)
NumPy
Matplotlib
tifffile
osgeo (GDAL)
scikit-learn

# Data  
Input Images Shape were 306 images each with (128,128,12)
while Labels shape were (128,128)

# Data Preparation
Dataset: Place your dataset of TIFF images and corresponding masks in a directory.

Data Loading: The dataset should be organized with input images and labels in separate arrays.

Normalization: Data normalization is applied to scale the pixel values.

Data Augmentation: The dataset is augmented to increase its diversity. The augmentation techniques include random flips, rotations, brightness, and contrast adjustments.

# Model Architecture
The model is based on the U-Net architecture, a popular choice for image segmentation tasks. The U-Net model includes:

Encoder: Down-sampling path that extracts features.
Bottleneck: Connects the encoder and decoder paths.
Decoder: Up-sampling path that reconstructs the segmentation masks.
Skip Connections: Connects encoder and decoder layers to preserve spatial information.



