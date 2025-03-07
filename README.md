# Webcam Motion Alert
A simple Python-based webcam application that monitors your webcam feed, detects motion, and sends an email alert when movement is detected.

## Features
Motion Detection: Uses OpenCV to compare the current video frame with a baseline frame for detecting motion.
Email Alerts: Captures an image when motion is detected and sends it via email using a custom emailing module.
Automatic Cleanup: Removes captured images from the folder after sending the alert.

## Requirements
Python 3.x
OpenCV (opencv-python)
A custom emailing module that contains the send_email function (configure it with your email settings).

## Installation
Clone the Repository:

git clone https://github.com/your-username/webcam-motion-alert.git
cd webcam-motion-alert

### Install Dependencies:
pip install opencv-python
Email Module Setup:

Ensure you have an emailing.py file in the project directory.
Configure the send_email function within it to use your email credentials and settings.

### Usage
Run the Application:
python main.py

Operation:

The app will open two windows: one showing the motion detection output and the other displaying the original video feed.
When motion is detected, an image is captured and an email alert is sent.
Press q to exit the application.

## Customization
Email Configuration: Update your emailing.py file with the correct credentials to ensure email alerts work.
Motion Detection Sensitivity: Adjust the contour area threshold (currently set to 5000) in the code to better suit your environment.
