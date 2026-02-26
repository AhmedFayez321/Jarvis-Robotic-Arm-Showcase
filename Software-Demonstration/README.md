# 🖥️ Jarvis Control Hub: The Core Software Ecosystem

This folder showcases the **Jarvis Desktop Suite**, a high-performance control center developed in Python. It acts as the primary interface between the user's commands (AI or Manual) and the robotic hardware.

## 📊 Dashboard Overview
The interface is designed using **CustomTkinter** for a modern, responsive user experience. It handles multi-threaded processes to ensure that AI vision tasks and mechanical movements never interrupt the GUI's responsiveness.

![Main Dashboard](./Photos/dashboard_interface.png)

*(Figure 1: The central control interface for Jarvis)*

---

## 🚀 Key Functional Features Explained

### 1. 🕹️ Hybrid Mobility & Arm Control
The software provides a dual-control mapping system:
* **Base Movement (L298 Integration):** Using the `W, A, S, D` keys, the software sends real-time signals to the motor drivers, allowing Jarvis to move in all directions.
* **6-DOF Precision:** Every joint of the arm is monitored. The dashboard displays real-time angles, ensuring the user always knows the robot's exact physical state.
* **Smart Gripper Toggle:** A dedicated logic for the gripper (`clos_open`) allows for seamless object manipulation with a single click or keypress.

### 2. 🎬 The Animation Recorder (Motion Capture)
This is the most advanced module in the suite. Instead of hard-coding movements, I developed a system to "teach" the robot:
* **Frame Persistence:** Record specific poses and save them into `.json` sequence files.
* **Mathematical Smoothing:** The engine calculates **Linear Interpolation** between frames. If you move from 0° to 90°, the software generates smooth intermediate steps to prevent mechanical vibration.
* **Playback Engine:** Supports looping, speed adjustment, and variable delays, making Jarvis capable of performing complex "human-like" gestures and dances.

### 3. 🔊 Interaction & Sound Sync
The software triggers specific serial commands that activate the **MP3 Module** on the hardware side. 
* When clicking "Check Hands" or starting a "Game", the software ensures the robot's voice lines (e.g., *"Hey, my name is Jarvis"*) are perfectly synced with its mechanical "Hi" gesture.

### 4. 🔗 AI & Logic Bridge
From this dashboard, two main AI modules can be launched:
* **Vision Tracking:** Automatically maps webcam coordinates to servo PWM signals.
* **Game Mode:** Initiates the "Rock Paper Scissors" logic, where the software acts as the judge, player, and animator.

---

## 🛠️ Technical Implementation (Under the Hood)

* **PyFirmata2 Protocol:** Used for high-speed, low-latency communication with the Arduino Mega.
* **Multi-Threading:** The animation playback and AI processing run on background threads (`threading.Thread`) to keep the UI fluid at 60FPS.
* **JSON Serialization:** All robot "memories" and animations are stored in structured JSON, allowing for easy sharing of robot motion profiles.

## 📂 Files in this Folder
* `dashboard_interface.png`: A full view of the control suite.
* `angle_monitor.png`: (Optional) Close-up of the real-time servo feedback.

---
### 👨‍💻 Developed by:
**Ahmed Fayez** *Robotics & AI Enthusiast*
