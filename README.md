
# Cartoonify Image with OpenCV

Convert images into a cartoon style using OpenCV and matplotlib.

## Prerequisites

Install the required libraries:

```bash
pip install opencv-python-headless numpy matplotlib
```

## Usage

1. Place the image (e.g., `dog.jpg`) in the same directory as the script.
2. Run the script:

```bash
python cartoonify.py
```

## Code Overview

- Load the image using `cv2.imread()`.
- Convert to grayscale with `cv2.cvtColor()`.
- Apply median blur using `cv2.medianBlur()`.
- Detect edges with `cv2.Laplacian()` and invert.
- Create a binary mask with `cv2.threshold()`.
- Apply a bilateral filter using `cv2.bilateralFilter()`.
- Combine filtered image with edge mask using `cv2.bitwise_and()`.
- Display original and cartoon images with matplotlib.


```markdown
# Image Processing with OpenCV and matplotlib

This project demonstrates various image processing techniques using OpenCV and matplotlib.

## Prerequisites

Install the required libraries:

```bash
pip install opencv-python-headless numpy matplotlib
```

## Usage

1. Place the images (e.g., `Nature.jpg` and `doggy.jpg`) in the same directory as the script.
2. Run the scripts:

For the nature image:

```bash
python cartoonify.py
```

For the doggy image transformations:

```bash
python transform_image.py
```

## Code Overview

### Cartoonify Image

- Load the image using `cv2.imread()`.
- Convert to grayscale with `cv2.cvtColor()`.
- Apply median blur using `cv2.medianBlur()`.
- Detect edges with `cv2.Laplacian()` and invert.
- Create a binary mask with `cv2.threshold()`.
- Apply a bilateral filter using `cv2.bilateralFilter()`.
- Combine filtered image with edge mask using `cv2.bitwise_and()`.
- Display original and cartoon images with matplotlib.

### Nature Image Division

- Load the image using `cv2.imread()`.
- Convert the image to a numpy array.
- Divide the image into four quadrants.
- Display each quadrant using matplotlib with titles.

### Image Transformations

- Load the image using `cv2.imread()` and convert to RGB.
- Perform and display various transformations including translation, scaling, and rotation.

