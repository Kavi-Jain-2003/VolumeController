🎛️ AI Hand Gesture Volume Controller

An AI-based system volume controller that allows users to control their computer's volume using hand gestures detected through a webcam. The project uses Computer Vision and Machine Learning techniques with MediaPipe for hand tracking and OpenCV for real-time video processing.

Instead of pressing keyboard keys or using the mouse, the user can increase or decrease the system volume by changing the distance between their thumb and index finger.

🚀 Features
<ul>
<li>✋ Real-time hand tracking using AI</li>
<li>📷 Uses webcam feed to detect hand gestures</li>
<li>🔊 Control system volume with finger distance</li>
<li>📊 Displays volume percentage bar</li>
<li>⚡ Shows real-time FPS</li>
<li>🧠 Uses MediaPipe Hand Landmark Detection</li>
</ul>

🧠 How It Works
<ul>
<li>The webcam captures live video.</li>
<li>MediaPipe Hands detects hand landmarks (21 key points).</li>
The system tracks:
<li>Thumb tip (Landmark 4)</li>
<li>Index finger tip (Landmark 8)</li>
<li>The distance between these two points is calculated.</li>
<li>That distance is mapped to the system volume range using interpolation.</li>
<li>The volume is updated in real time using PyCAW.</li>
</ul>

***Thumb ↔ Index Finger Distance → Volume Level***
***Closer fingers → Lower volume***
***Farther fingers → Higher volume***

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
The system shows:Hand landmarks, Distance line between fingers, Volume percentage bar, Real-time FPS.

🔮 Future Improvements
<ul>
<li>Add mute gesture</li>
<li>Control brightness</li>
<li>Multi-hand gesture support</li>
<li>Cross-platform audio support</li>
<li>GUI interface</li>
</ul>

📚 Learning Outcomes:
Through this project, I learned:
<ol>
<li>Real-time computer vision processing</li>
<li>Hand landmark detection using MediaPipe</li>
<li>Mapping gesture distance to system-level controls</li>


👨‍💻 Author
Kavi Jain
Computer Applications Graduate
Interested in AI, Data Science, and Full Stack Development
