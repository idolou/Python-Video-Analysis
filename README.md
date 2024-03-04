# Video Analysis Project

This project aims to analyze videos using Python for various purposes such as detecting significant movement, identifying dominant colors, detecting faces, and recognizing text within the frames. Below is a breakdown of the functionalities provided by this project:

## Features

### Brightest and Darkest Frames Detection
- Utilizes OpenCV to identify the brightest and darkest frames within the video.
- Calculates the average brightness of each frame and compares them to determine the brightest and darkest frames.

### Color Dominance Analysis
- Analyzes the color dominance in a video by computing the average value of each color channel (Red, Green, Blue) across all frames.
- Identifies the frame with the highest average value for each color channel.

### Movement Detection
- Detects significant movement in a video by comparing consecutive frames.
- Allows users to specify a threshold value and the minimum number of pixels changed to consider it as significant movement.

### Face Detection
- Detects faces in each frame of a video using the Haar cascade classifier for face detection.
- Provides the number of faces detected and highlights them with green rectangles in the frames.

### Text Recognition
- Utilizes OCR (Optical Character Recognition) to recognize and extract text from frames in a video.
- Applies Tesseract OCR to perform text recognition on each frame.

## Installation

Before running the project, make sure to install the required libraries by executing the following commands:

```python
!apt-get install tesseract-ocr
!pip install pytesseract
```


## Usage

1. Upload a video file using the provided script.
2. Choose from the available functionalities to analyze the video.
3. Follow the instructions in each section to perform specific analysis tasks.

## Example Usage

To perform text recognition on a video, use the following script to upload the video file:

```python
uploaded_file = files.upload()
file_name = next(iter(uploaded_file))
video_path = f"/content/{file_name}"
```

## Requirements

- Python 3.x
- OpenCV
- moviepy
- numpy
- matplotlib
- pytesseract
- Google Colab (for running the notebook)
