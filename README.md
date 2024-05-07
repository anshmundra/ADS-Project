## Overview
This project explores how to effectively implement and possibly improve upon existing models for digit classification in complex, real-world images. We use the Street View House Numbers (format 1) dataset Our focus is on preprocessing data, building and comparing different CNN models, and experimenting with complex object detection frameworks like YOLO.

## Contents
1. **Data Preprocessing**
   - This section deals with preparing the data for modeling. It includes categorical conversion, normalizing, and splitting the dataset.
   
2. **Model 1 Building**
   First simple CNN:
      **Initial Convolution and Pooling**:
     - `Conv2D`: 64 filters, 3x3, ReLU activation, input shape (32, 32, 3)
     - `AveragePooling2D`: 2x2, reduces spatial dimensions while retaining important features
   
        **Second Convolutional Block**:
     - `Conv2D`: 128 filters, 3x3, ReLU activation, padding 'same'
     - `BatchNormalization`: Normalizes the activations from the previous layer, improving stability
     - `MaxPooling2D`: 2x2, further reduces dimensionality and helps to prevent overfitting
   
        **Third Convolutional Block**:
     - `Conv2D`: 256 filters, 3x3, ReLU activation, padding 'same'
     - `MaxPooling2D`: 2x2, sharpens the features for the final classification
     - `Dropout`: 0.4, significantly reduces overfitting by randomly turning off a fraction of neurons

   
3. **Model 2 Building**
   
   Built a more complex CNN with this architecture:
   
      - **Block 1**: Two convolutional layers with 32 filters
      - **Block 2**: Two convolutional layers with 64 filters
      - **Block 3**: Two convolutional layers with 128 filters
      - Dropout and Max Pooling are applied sequentially in each block.
   
5. **YOLO Implementation Attempt**
   - An exploratory section where we attempt to implement the YOLOv7 model (https://github.com/WongKinYiu/yolov7) for object detection.

## Usage
To run this notebook:
1. Ensure you have Jupyter Notebook or JupyterLab installed.
2. Clone/download this repository.
3. Navigate to the project directory.
4. Run `jupyter notebook` or `jupyter lab` and open the `ADS_Project_Ansh_x_Dhiren.ipynb` file.
5. Download Format 1 of the Street View House Numbers Dataset (http://ufldl.stanford.edu/housenumbers/).

## Requirements
- Python 3.x
- TensorFlow
- NumPy
- Matplotlib

## Contributors
- Ansh Mundra
- Dhiren Shivdasani
