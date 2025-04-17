🤖 Body Detection with Smart Dog Robot
This project introduces a smart robot dog system developed to detect people trapped under debris in *disaster scenarios, especially **earthquakes, and to support rescue teams. The system uses the *YOLO (You Only Look Once) object detection algorithm for visual recognition, and robot movement is achieved via Wi-Fi-controlled servo motors.

🚀 Features
🔍 Real-time person detection using YOLOv8
🎥 Live video stream via computer camera (Raspberry Pi integration planned)
🧠 AI-based decision-making system
📡 Wireless control using ESP8266 (NodeMCU)
⚙ Multi-axis movement with servo motors
🤸‍♂ Pre-programmed actions: move forward, do push-ups, standby mode
🛠 Technologies Used
Python (OpenCV, socket, Ultralytics YOLOv8)
Arduino (ESP8266 & Servo libraries)
YOLOv8 (Ultralytics)
ESP8266 Wi-Fi module (NodeMCU)
Raspberry Pi (for future development)
🖥 System Architecture
Python side: Captures video from the computer camera, detects humans using YOLO, and sends commands to ESP8266 based on detection results.
ESP8266 side: Executes servo motor movements based on received commands (e.g., move forward, idle, do push-ups).
Future goal: Replace computer camera with Raspberry Pi camera for a fully embedded system.
🔧 How to Use
Install the required Python packages: bash pip install opencv-python ultralytics numpy

Load the YOLOv8 model: python from ultralytics import YOLO model = YOLO('yolov8n.pt')

Upload the ESP8266 code via Arduino IDE:

Check the servo pin mappings.
Enter your Wi-Fi SSID and password.
Run the Python script: bash python smart_dog.py

Once a person is detected via the camera, the robot starts moving accordingly 🚶‍♂

📌 Future Plans
📷 Integrate Raspberry Pi camera module
🌐 Remote control via Internet connection
🧭 Environmental mapping and obstacle detection
🔊 Voice command integration
🤝 Contribute
Contributions and pull requests are always welcome! Feel free to report bugs, suggest improvements, or join in on development 🙌
