# Live Face Recognition

A Python-based real-time face recognition system that uses computer vision to detect and recognize faces through a webcam feed.

## Overview

This project implements live face recognition using OpenCV and face_recognition libraries in Python. It captures video from your webcam, detects faces in real-time, and can recognize known faces based on pre-trained data.

## Requirements

- Python 3.6+
- OpenCV (`cv2`)
- face_recognition
- numpy

Install the required packages using:

```bash
pip install opencv-python face_recognition numpy
```

## Technical Concepts

The main.py file utilizes several important concepts:

### 1. OpenCV (cv2)
- Used for capturing video feed from webcam
- Handles image processing and display
- Provides drawing utilities for rectangles and text on frames

### 2. face_recognition Library
- Provides face detection capabilities
- Handles face encoding (converting facial features into numerical data)
- Performs face comparison and recognition

### 3. Key Functions

#### Face Detection
- Uses HOG (Histogram of Oriented Gradients) for face detection
- Converts frames to RGB color space for processing
- Returns locations of faces in frames

#### Face Recognition
- Creates face encodings (128-dimensional vectors)
- Compares face encodings with known faces
- Uses distance calculations to determine matches

#### Real-time Processing
- Captures frames from webcam in real-time
- Processes each frame for face detection
- Updates display with recognition results

## Usage

1. Clone the repository:
```bash
git clone https://github.com/ashish0ct/Live_Face_Recognition.git
cd Live_Face_Recognition
```

2. Run the main script:
```bash
python main.py
```

3. The webcam will activate and begin detecting faces in real-time.

## How It Works

1. The system captures video frames from your webcam
2. Each frame is processed to detect faces
3. Detected faces are encoded into numerical data
4. These encodings are compared with known face encodings
5. Results are displayed in real-time on the video feed

## Performance Considerations

- Face detection and recognition are CPU-intensive operations
- Processing speed depends on:
  - Hardware capabilities
  - Number of faces in the frame
  - Frame resolution
  - Lighting conditions

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
