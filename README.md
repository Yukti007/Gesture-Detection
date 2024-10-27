# Hand Gesture Volume Control

This project is a **hand gesture-controlled volume adjustment system**. Using **OpenCV** and **MediaPipe**, the program detects hand gestures and adjusts the system's audio volume based on the movement and position of the thumb and index fingers. The code is optimized for real-time response with low latency, making it adaptable for diverse lighting and movement conditions.

## Features
- **Volume Control:** Adjust volume by moving your hand up or down.
- **Real-time Hand Detection:** Uses MediaPipe's pre-trained hand detection model.
- **Custom Sensitivity & Scaling:** Easily adjust sensitivity and scaling for precise volume changes.

## Requirements
- **Python 3.x**
- **Required Libraries:** 
  - OpenCV (`cv2`)
  - MediaPipe
  - Numpy
  - Pycaw (for Windows audio control)

To install the libraries, run:

pip install opencv-python mediapipe numpy pycaw comtypes
## Usage
Run the Code:
python hand_volume_control.py

Adjust Volume:
Place your thumb and index finger in front of the webcam.
Move your hand up to increase and down to decrease the volume.
Press q to quit the application.

## How It Works
Hand Detection: Uses MediaPipe's Hands module to detect hand landmarks.
Volume Control Logic:
Measures the distance between the thumb and index finger.
Determines vertical movement of the hand to adjust volume up or down.
Volume Adjustment: Volume change is proportional to finger distance and movement speed, making it responsive yet controllable.

## Parameters
Sensitivity: Controls how quickly the program detects hand movement direction.
Scaling Factor: Adjusts the rate of volume change for smooth control.
## Troubleshooting
If you encounter an ImportError, verify all required libraries are installed.


To install all dependencies from this file, run:
pip install -r requirements.txt
