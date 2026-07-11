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
Installation
1. Clone the repository
git clone https://github.com/your-username/AttendEye.git
cd AttendEye
2. Create a virtual environment (Optional)
python -m venv venv

Activate the environment:

Windows

venv\Scripts\activate

Linux/macOS

source venv/bin/activate
3. Install dependencies
pip install -r requirements.txt

Or install manually:

pip install opencv-python mediapipe ultralytics numpy
4. Download YOLOv8 model

The model will automatically download the first time you run the project. Alternatively, download yolov8n.pt and place it in the project folder.

5. Run the project
python app.py
Project Structure
AttendEye/
│── app.py
│── yolov8n.pt
│── database/
│   └── attention.db
│── screenshots/
│── requirements.txt
└── README.md
Output

The application provides:

Live webcam monitoring
Attention score
Face detection status
Blink count
Yawn count
Head direction
Mobile phone detection
Liveness status
Attention dashboard
SQLite database logs
Screenshots of low-attention events
