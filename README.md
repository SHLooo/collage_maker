# collage_maker

The `create_collage.ipynb` notebook is a demonstration of how to create a customized photo collage of any shape using Python. This tool allows you to provide a silhouette of the desired shape, and it will generate a collage with photos that conform to the shape.

## Backstory
https://www.linkedin.com/posts/shuhao-uw_opencv-numpy-uwaterloo-activity-7078657845252034561-2vOW?utm_source=share&utm_medium=member_desktop

## Packages
- cv2
- matplotlib.pyplot
- numpy
- os

## Features
- Supports custom shapes: You can provide a silhouette of the desired shape for the collage.
- Thresholding: The silhouette is separated into object pixels and background pixels using a tunable threshold.
- Grid division: The collage is divided into a grid of square cells, with the option to specify the cell width.
- Photo placement: Photos are placed in the grid cells, representing the shape in a pixelated manner.
- Batch creation: Two batches of photos are created for the shape - one at the border and one inside the shape.
- Border definition: The border is determined by the percentage of the shape in a given grid cell, with a tunable threshold (defaulted to 75%).
- Cell spacing: There is a customizable border of 15 pixels between each grid cell.
- Masking: The photos are masked using the thresholded silhouette to conform to the exact shape.

## Input Requirements
- Supported image formats: The photos used to fill the collage must be in either .jpg or .png format.
- Photo resizing: The photos will be reshaped to a square by cropping on one axis and then resized to match the cell size.
- RGB color representation: The photos and the collage are assumed to use RGB color representation.
Setup and Parameters
- Please refer to the Setups and Parameters section within the notebook. It provides a complete list of inputs and tunable parameters that you can adjust to customize your photo collage.
- Note: It is recommended to have slightly fewer photos than required to avoid excessive duplicates while utilizing all your available photos effectively.

## Data

A total of 473 photos are uploaded in the GitHub repo. This should be enough to create a photo collage with any shape and dimension. If not, please comment below.
