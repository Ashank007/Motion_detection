# Motion Detection using OpenCV

## Description
This Python script captures video from the webcam and detects motion by comparing the current frame to the first frame or the frame taken every 30 frames. It highlights the detected motion areas with rectangles.

## Requirements
Python 3.x

OpenCV (cv2)

## Installation

Install Python 3.x from the official Python website.

Install OpenCV by running the following command:

```bash
pip install opencv-python
```
## Usage
Save the script to a file, for example motion_detection.py.

Run the script using Python:

```bash
python motion_detection.py
```
The script will start capturing video from the webcam. Press 'q' to quit the application.

## How It Works
Capture Video: The script captures video from the default webcam using cv2.VideoCapture(0).

Convert to Grayscale and Blur: Each frame is converted to grayscale and blurred to reduce noise and improve motion detection accuracy.

Frame Comparison: The script compares the current frame to the first frame or the frame taken every 30 frames to detect changes (motion).

Threshold and Contours: The difference between frames is thresholded to create a binary image highlighting motion areas. Contours are then found to detect the regions with motion.

Draw Rectangles: For each contour that has an area greater than a specified threshold, a rectangle is drawn around the detected motion area.

Display Frame: The current frame with detected motion areas highlighted is displayed in a window.

Exit: Press 'q' to exit the application and release the webcam.

## Example

Run the script and move in front of your webcam. The motion areas will be highlighted with rectangles.

