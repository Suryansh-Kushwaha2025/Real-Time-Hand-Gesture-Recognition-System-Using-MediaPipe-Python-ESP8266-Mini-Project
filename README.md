# Real-Time-Hand-Gesture-Recognition-System-Using-MediaPipe-Python-ESP8266-Mini-Project
A real-time hand gesture recognition system using MediaPipe, OpenCV, and Python, integrated with ESP8266 and a 16×2 I2C LCD. The system detects hand landmarks via webcam, recognizes gestures, and displays results on hardware, enabling low-cost, touchless human–machine interaction for IoT applications.
This repository contains the complete implementation of a real-time hand gesture recognition system that enables touchless human–machine interaction using computer vision and embedded systems. The project leverages MediaPipe, OpenCV, and Python for accurate hand detection and gesture classification, and integrates the recognized gestures with an ESP8266 microcontroller to display outputs on a 16×2 I2C LCD.

The system works by capturing live video input from a standard webcam. MediaPipe Hands is used to detect and track 21 hand landmarks in real time, even under varying lighting conditions. Based on the relative positions and angles of these landmarks, custom logic is applied in Python to recognize predefined hand gestures such as fist, palm, thumbs-up, peace sign, and others. A stability filter ensures that only consistent gestures are transmitted, reducing noise and false detections.

Once a gesture is recognized, the data is sent from the Python application to the ESP8266 via serial communication over USB. The ESP8266 processes this data and displays the corresponding gesture message on an LCD screen using the I2C protocol, which simplifies wiring and reduces hardware complexity. This demonstrates effective software–hardware integration, bridging AI-based vision processing with real-world embedded output.

The project is designed to be low-cost, lightweight, and beginner-friendly, requiring no GPU or specialized sensors—only a webcam and commonly available components. Its modular structure allows easy extension, such as adding new gestures, controlling external devices (relays, motors, robots), or integrating IoT platforms like Blynk or MQTT.

This system has potential applications in assistive technology, smart homes, contactless control systems, industrial automation, and human–computer interaction research. It also serves as an excellent academic mini/major project for students interested in AI, IoT, embedded systems, and computer vision.

The repository includes source code, hardware connection details, and setup instructions to help users understand, run, and extend the project efficiently.
