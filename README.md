# Image as Data

## Aim
To read, write, and explore image data.

## Introduction
Image data is commonly used to represent graphic or pictorial information. It consists of pixel-based representations that can be created, collected, and stored using image constructor devices. Various industry-standard formats, such as TIFF, GIF, and PCX, are used to store image data, making it accessible for different software applications, including GIS and image processing systems.

This project provides extensive examples and introduces the essential Python libraries required for image processing. It covers fundamental operations such as reading, converting, plotting, and saving images.

## Libraries for Image Processing

### 1. **PIL (Python Imaging Library)**
PIL provides essential image-handling capabilities, including resizing, cropping, rotating, and color conversion. It allows easy manipulation of image data within Python. The library has been superseded by Pillow, a modern, user-friendly fork.

- Official website: [PythonWare - PIL](http://www.pythonware.com/products/pil/)
- Pillow is maintained by Alex Clark and contributors.

### 2. **Scikit-Image**
Scikit-Image is a collection of algorithms for image processing and computer vision. It offers numerous utilities for image manipulation, enhancement, and analysis. Below are some key subpackages:

- **color**: Color space conversion.
- **data**: Test images and example datasets.
- **draw**: Functions for drawing primitives like lines and text.
- **exposure**: Adjusting image intensity and histogram equalization.
- **feature**: Feature detection and extraction, including texture analysis.
- **filters**: Sharpening, edge detection, and thresholding.
- **graph**: Graph-based image processing.
- **io**: Image and video file reading, saving, and display.
- **measure**: Extracting image properties and contours.
- **metrics**: Distance and similarity metrics for images.
- **morphology**: Morphological operations like opening and skeletonization.
- **restoration**: Algorithms for image denoising and deconvolution.
- **segmentation**: Partitioning images into multiple regions.
- **transform**: Geometric transformations such as rotation.
- **util**: General utility functions for image processing.
- **viewer**: A simple GUI for visualizing and modifying images.

## Key Features of the Project
- Reading and writing images using Python libraries.
- Converting images between different formats.
- Performing basic image processing operations like resizing and filtering.
- Visualizing image transformations using various Python tools.

## Installation
To use the libraries in this project, install the required dependencies using:

```sh
pip install pillow scikit-image
```

## Usage
Import the necessary libraries and perform basic image processing tasks:

```python
from PIL import Image
from skimage import io, color

# Load an image
image = Image.open("example.jpg")
image.show()

# Convert to grayscale
gray_image = image.convert("L")
gray_image.show()

# Using Scikit-Image to read and display an image
img = io.imread("example.jpg")
io.imshow(img)
```

## Conclusion
This project provides a foundational understanding of handling image data using Python. It explores key image processing libraries, demonstrating how to read, write, and manipulate images efficiently.

## References
- [Pillow Documentation](https://pillow.readthedocs.io/)
- [Scikit-Image Documentation](https://scikit-image.org/)
