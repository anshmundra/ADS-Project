## Overview
This project explores how to effectively implement and possibly improve upon existing models for digit classification in complex, real-world images. Our focus is on preprocessing data, building and comparing different CNN models, and experimenting with complex object detection frameworks like YOLO.

## Contents
1. **Data Preprocessing**
   - This section deals with preparing the data for modeling. It includes categorical conversion, normalizing, and splitting the dataset.
   
2. **Model 1 Building**
   - Here, we develop our first CNN model.
   
3. **Model 2 Building**
   - Built a more complex CNN with this architecture:
      - **Block 1**: Two convolutional layers with 32 filters
      - **Block 2**: Two convolutional layers with 64 filters
      - **Block 3**: Two convolutional layers with 128 filters
      - Dropout and Max Pooling are applied sequentially in each block.
   
4. **YOLO Implementation Attempt**
   - An exploratory section where we attempt to implement the YOLO model for object detection.

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
