# Baby_Monitor_Raspberry_Pi
IoT Baby Monitor built with Raspberry Pi: real-time audio detection, Flask video streaming, and automated email alerts.



A smart 👶� baby-monitoring system built using Raspberry Pi, capable of:


🎤 Detecting baby cries using live audio

📸 Capturing images when crying is detected

🌐 Streaming live video through a Flask MJPEG server

📧 Sending email alerts with a link to the live stream

This project was built using Python, Flask, sounddevice, and Raspberry Pi camera tools.



🚀 Features

🔊 1. Cry Detection
Uses the microphone to continuously listen.
Calculates volume using NumPy.
Detects cry/noise above a threshold.
Triggers an alert event.

📸 2. Automatic Image Capture
When a cry is detected:
Raspberry Pi camera runs rpicam-still
Saves an image with timestamp.

📧 3. Email Alert Notification
Sends an email via SMTP.
Includes:
Message alert
Clickable link to live video stream

📺 4. Live Video Streaming
Flask server streams stream.jpg using MJPEG.
Another script continuously updates the frame.
