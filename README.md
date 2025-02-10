# Traffic Maestro
 An OpenCV-based vehicle detection and counting system using background subtraction and contour detection.
## Vehicle Detection and Counting Using OpenCV

This project is a simple vehicle detection and counting system using OpenCV and Python. It processes a video file to detect and count moving vehicles using background subtraction and contour detection.

## Features

Detects and counts vehicles in a given video.

Uses background subtraction and morphological operations for better accuracy.

Displays bounding boxes and a counting line to track vehicles.

Outputs the total count of detected vehicles in real-time.

## Prerequisites

Make sure you have the following installed:

Python 3.x

OpenCV

NumPy

You can install the required dependencies using:

pip install opencv-python numpy

## Usage

Place the video file in the appropriate directory.

Update the cap = cv2.VideoCapture("/path/to/video.mp4") line in main.py with the correct video file path.

Run the script:

python main.py

The script will start detecting and counting vehicles in real-time.

Press ESC to stop the program.

## Code Explanation

The script reads frames from the video and applies frame differencing to detect moving objects.

It converts frames to grayscale, applies Gaussian blur, and performs morphological transformations to clean up noise.

Contours are extracted to detect vehicle-like shapes.

Vehicles crossing a predefined line are counted and displayed on the screen in real-time.

## Project Structure

|-- vehicle_detection
    |-- main.py  # Main script for vehicle detection and counting
    |-- README.md  # Project documentation

## Future Improvements

Enhance vehicle tracking to prevent double counting.

Improve accuracy using deep learning-based object detection models like YOLO.

Implement real-time processing with a live camera feed.



