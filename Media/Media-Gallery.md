# 🎞️ Jarvis Live Demonstration & Media Gallery

This gallery provides a visual journey of the **Jarvis Robotic System**, showcasing its transition from a technical prototype to an interactive AI entity at public exhibitions.

---

## 📽️ Video Demonstrations

### 🎮 1. Full System Integration & Wireless Control
This video is the most comprehensive look at Jarvis's capabilities.
* **Key Features:** Manual operation via the **Custom Wireless Controller**, real-time telemetry on the **OLED Screen**, and the **Serial MP3 Module** providing Jarvis with a voice.
* **Technical Note:** Notice the low-latency response between the NRF24L01 wireless modules.
* `[Watch Video: Controller & Voice Demo](./Media/videos/system_overview.mp4)`

### ✊✋✌️ 2. The Exhibition Highlight: Rock-Paper-Scissors
Filmed during a live tech conference, Jarvis competes against human opponents autonomously.
* **The Logic:** Watch as Jarvis initiates the countdown, captures the user's gesture via the webcam, and uses its **AI Decision Engine** to play and react (Victory/Defeat animations).
* `[Watch Video: Live RPS Game Mode](./Media/videos/rps_conference.mp4)`

### 🎯 3. Autonomous Vision Tracking (Nose-Lock)
A demonstration of the robot's ability to maintain "social presence."
* **Mechanism:** Jarvis uses **MediaPipe Pose Tracking** to lock onto the user's nose coordinates. The system then maps these pixels to servo degrees, ensuring the robot's base follows the user smoothly.
* `[Watch Video: AI Vision Tracking](./Media/videos/tracking_demo.mp4)`

### 🤝 4. Social Interaction: The Handshake
Jarvis performing a friendly "Human-like" greeting animation.
* **Smoothing:** This video highlights the **Linear Interpolation** logic in the animation engine, showing fluid mechanical motion without jitter.
* `[Watch Video: Greeting & Handshake](./Media/videos/greeting_demo.mp4)`

---

## 📸 Photo Gallery

### 🏢 Public Exhibition & Presentation
Moments captured during the conference presentation. These photos showcase the interaction between the developer, the audience, and Jarvis, explaining the complex AI and Embedded logic behind the build.

<p align="center">
  <img src="./Media/images/conference_1.png" width="32%" alt="Conference Presentation 1">
  <img src="./Media/images/conference_2.png" width="32%" alt="Conference Presentation 2">
  <img src="./Media/images/conference_3.pmg" width="32%" alt="Conference Presentation 3">
</p>

---

### 🦾 Hardware Synergy
A high-resolution shot of the complete ecosystem—the 6-DOF Robotic Arm and its dedicated Wireless Command Unit.

![Jarvis and Controller](./Media/images/full_setup.png)
*Figure 1: The dual-unit robotics solution: Precision hardware meets Intelligent software.*

---

## 📂 Media Organization
To ensure all assets are linked correctly, please maintain the following structure:
```text
/Media
 ├── /videos
 │    ├── system_overview.mp4
 │    ├── rps_conference.mp4
 │    ├── tracking_demo.mp4
 │    └── greeting_demo.mp4
 └── /images
      ├── conference_1.jpg
      ├── conference_2.jpg
      ├── conference_3.jpg
      └── full_setup.jpg

### 👨‍💻 Developed by:
**Ahmed Fayez** *Robotics & AI Systems Developer*
