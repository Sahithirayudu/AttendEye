AttendEye – AI-Powered Student Attention Monitoring System

AttendEye is a real-time AI-based student attention monitoring system that analyzes a student's attentiveness using computer vision. It detects face presence, head pose, eye blinks, yawning, mobile phone usage, and possible spoofing attempts while maintaining an attention score. The system also stores attention logs in a SQLite database and captures screenshots whenever low-attention events occur.

Features
Real-time face detection using MediaPipe
Face landmark detection for eye and mouth tracking
Head pose estimation (Left, Right, Up, Down, Forward)
Blink and drowsiness detection
Yawn detection
Mobile phone detection using YOLOv8
Liveness verification using blink and movement analysis
Attention score calculation
Live dashboard displaying attention metrics
Automatic screenshot capture for low-attention events
SQLite database logging with timestamps
Technologies Used
Python
OpenCV
MediaPipe
YOLOv8 (Ultralytics)
NumPy
SQLite
