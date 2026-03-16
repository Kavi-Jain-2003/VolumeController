🎛️ AI Hand Gesture Volume Controller

An AI-based system volume controller that allows users to control their computer's volume using hand gestures detected through a webcam. The project uses Computer Vision and Machine Learning techniques with MediaPipe for hand tracking and OpenCV for real-time video processing.

Instead of pressing keyboard keys or using the mouse, the user can increase or decrease the system volume by changing the distance between their thumb and index finger.

🚀 Features

✋ Real-time hand tracking using AI

📷 Uses webcam feed to detect hand gestures

🔊 Control system volume with finger distance

📊 Displays volume percentage bar

⚡ Shows real-time FPS

🧠 Uses MediaPipe Hand Landmark Detection

🧠 How It Works

The webcam captures live video.

MediaPipe Hands detects hand landmarks (21 key points).

The system tracks:

Thumb tip (Landmark 4)

Index finger tip (Landmark 8)

The distance between these two points is calculated.

That distance is mapped to the system volume range using interpolation.

The volume is updated in real time using PyCAW.

Thumb ↔ Index Finger Distance → Volume Level


Closer fingers → Lower volume
Farther fingers → Higher volume

🛠️ Technologies Used

Python

OpenCV

MediaPipe

NumPy

PyCAW (Python Core Audio Windows Library)

Computer Vision

📂 Project Structure
AI-Hand-Gesture-Volume-Control/
│
├── HandTrackingModule.py      # Hand detection and landmark tracking module
├── VolumeHandControl.py       # Main program to control system volume
└── README.md                  # Project documentation

⚙️ Installation
1️⃣ Clone the Repository
git clone https://github.com/Kavi-Jain-2003/VolumeController.git
cd VolumeController

2️⃣ Install Dependencies
pip install opencv-python mediapipe numpy pycaw comtypes

▶️ Run the Project
python VolumeHandControl.py


Press Q to exit the program.

✋ Gesture Control
Gesture	Action
Thumb & Index Finger Close	Decrease Volume
Thumb & Index Finger Far	Increase Volume

📊 Output

The system shows:

Hand landmarks

Distance line between fingers

Volume percentage bar

Real-time FPS

🔮 Future Improvements

Add mute gesture

Control brightness

Multi-hand gesture support

Cross-platform audio support

GUI interface

📚 Learning Outcomes

Through this project, I learned:

Real-time computer vision processing

Hand landmark detection using MediaPipe

Mapping gesture distance to system-level controls

Integrating Python with OS audio APIs

👨‍💻 Author

Kavi Jain

Computer Applications Graduate

Interested in AI, Data Science, and Full Stack Development
