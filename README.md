Hand Gesture Recognition System
This repository contains a Python application for real-time hand gesture recognition using the MediaPipe library. The system detects and tracks hand gestures from a live video feed and performs gesture classification for various hand poses and movements.

Requirements
Python 3.x
OpenCV (cv2)
NumPy
Mediapipe
Other dependencies specified in requirements.txt
Installation
Clone the repository to your local machine:

bash
Copy code
git clone https://github.com/yourusername/your-repo.git
Install the required Python packages:

Copy code
pip install -r requirements.txt
Usage
Navigate to the directory containing the cloned repository.

Run the main Python script:

Copy code
python hand_gesture_recognition.py
Use the following keys for interaction:

Press ESC to exit the application.
Press n to enter logging mode for capturing key points.
Press k to enter logging mode for capturing point history.
Press h to exit logging mode.
Press 0 to 9 to specify the gesture number during logging.
Perform hand gestures in front of the camera to trigger gesture recognition and classification.

Files
hand_gesture_recognition.py: The main Python script for real-time hand gesture recognition.
model: Directory containing the trained models for keypoint classification and point history classification.
utils.py: Utility functions for FPS calculation and other helper functions.
model.py: Python files defining the keypoint classifier and point history classifier classes.
README.md: Instructions and information about the hand gesture recognition system.

# Directory
<pre>
│  app.py
│  keypoint_classification.ipynb
│  point_history_classification.ipynb
│  
├─model
│  ├─keypoint_classifier
│  │  │  keypoint.csv
│  │  │  keypoint_classifier.hdf5
│  │  │  keypoint_classifier.py
│  │  │  keypoint_classifier.tflite
│  │  └─ keypoint_classifier_label.csv
│  │          
│  └─point_history_classifier
│      │  point_history.csv
│      │  point_history_classifier.hdf5
│      │  point_history_classifier.py
│      │  point_history_classifier.tflite
│      └─ point_history_classifier_label.csv
│          
└─utils
    └─cvfpscalc.py
</pre>

Acknowledgments
This project utilizes the MediaPipe library for hand tracking and gesture recognition.
The models used for gesture classification are trained using custom datasets.
Author
Ashwanthram A.C