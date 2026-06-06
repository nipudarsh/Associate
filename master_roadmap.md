# 🚀 THE UNIFIED 9-MONTH MASTER ROADMAP  
## "From Foundation to Untouchable Associate Engineer"  
  
This document integrates the **Execution Blueprint**, **Hardware Shopping Lists**, and the **Free Resource Master Guide** into a single, cohesive, phase-by-phase execution plan.  
  
---  
  
# 🛠️ PRE-REQUISITES: ENVIRONMENT & TOOLS SETUP  
*(Complete these before starting Month 1)*  
  
**1. Core Software Installation (All Free):**  
*   **VS Code (Main IDE):** [Download](https://code.visualstudio.com/download)  
    *   *Extensions:* PlatformIO IDE, C/C++ (Microsoft), Python, GitLens.  
*   **PlatformIO IDE:** [Setup Guide](https://platformio.org/install/ide?install=vscode) | [Video Tutorial](https://www.youtube.com/watch?v=0poh_2rBq7E)  
*   **Git & GitHub Desktop:** [Git Download](https://git-scm.com/downloads) | [GitHub Desktop](https://desktop.github.com/)  
*   **Notion (For Tracking):** [Signup](https://www.notion.so/signup) (Create a daily learning log and project tracker).  
  
---  
  
# 🟡 PHASE 1: "THE FOUNDATION FORGE" (Months 1-3)  
**Goal:** Build unshakable fundamentals + First 2 flagship projects.  
  
## 🛒 Phase 1 Hardware & Components Needed:  
*   **Microcontrollers:** ESP32 DevKit (x3)  
*   **Robot Parts:** 2WD/4WD Chassis kit, Motor encoders (x2), L298N motor driver, Servo motor SG90 (x2).  
*   **Sensors:** MPU6050 IMU, HC-SR04 ultrasonic (x3), DHT22 Temp/Humidity (x3).  
*   **Misc:** Breadboards, jumper wires, LED assortment, resistors, power supply (5V/3A).  
  
---  
  
## 📅 MONTH 1: EMBEDDED CORE MASTERY  
  
### Week 1-2: FreeRTOS Deep Dive  
**Tasks:**  
*   Learn Task creation, Priorities, Queues, Semaphores, Timers, Interrupts, Memory Management.  
*   Write 5 working examples on the ESP32 (LED blink, sensor read, passing data via queues).  
  
**Guidance & Resources:**  
*   📺 **Main Course:** [Shawn Hymel's FreeRTOS ESP32 Series (12 episodes)](https://www.youtube.com/playlist?list=PLEBQazB0HUyQ4hAPU1cJED6t3DU0h34bz)  
*   📘 **Reading:** [Mastering the FreeRTOS Kernel (Free PDF)](https://www.freertos.org/Documentation/Mastering-the-FreeRTOS-Real-Time-Kernel.v1.0.pdf)  
  
### Week 3-4: PID Control Systems & Motor Control  
**Tasks:**  
*   Understand PID mathematically (Proportional, Integral, Derivative).  
*   Implement DC motor speed control with an encoder (read pulses via interrupt).  
*   Read MPU6050 data and apply a complementary filter.  
  
**Guidance & Resources:**  
*   📺 **Theory:** [Brian Douglas "PID Control" Playlist](https://www.youtube.com/playlist?list=PLUMWjy5jgHK1NC52DXXrriwihVrYZKqjk)  
*   📺 **Practical:** [PID Motor Speed Control](https://www.youtube.com/watch?v=fv6dLTEvl74)  
*   🎓 **Course:** [Modern Robotics (Coursera - Free Audit)](https://www.coursera.org/learn/modernrobotics-course1)  
  
---  
  
## 📅 MONTH 2: FLAGSHIP PROJECT 1 - AUTONOMOUS ROBOT  
**Project Goal:** Differential drive robot with FreeRTOS, PID control, and sensor fusion.  
  
### Week 1-4 Tasks:  
*   **Week 1 (Assembly):** Wire motors/encoders to L298N. Implement PID speed control for straight driving.  
*   **Week 2 (Sensors):** Integrate HC-SR04 (Ultrasonic) and MPU6050 (IMU) using FreeRTOS tasks.  
*   **Week 3 (Logic):** Build a State Machine (Forward, Scanning, Turning, Stopped). Implement obstacle avoidance.  
*   **Week 4 (Comms):** Add Bluetooth control via MIT App Inventor. Document everything on GitHub.  
  
**Guidance & Resources:**  
*   🔧 **Encoder Code:** [ESP32 Motor Encoder Guide](https://randomnerdtutorials.com/esp32-dc-motor-encoder/)  
*   🔧 **MPU6050 Setup:** [ESP32 + MPU6050](https://randomnerdtutorials.com/esp32-mpu-6050-accelerometer-gyroscope-arduino/)  
*   📱 **Bluetooth App:** [ESP32 Bluetooth Classic](https://randomnerdtutorials.com/esp32-bluetooth-classic-arduino-ide/)  
  
---  
  
## 📅 MONTH 3: FLAGSHIP PROJECT 2 - INDUSTRIAL IoT SYSTEM  
**Project Goal:** 3-Node ESP32 environmental monitoring network using MQTT and Grafana.  
  
### Week 1-4 Tasks:  
*   **Week 1 (Nodes):** Set up 3 ESP32s reading DHT22s. Publish to a Mosquitto MQTT Broker.  
*   **Week 2 (Database):** Install InfluxDB and Grafana. Create real-time dashboards.  
*   **Week 3 (Automation):** Use Node-RED to trigger alerts (Telegram/Email) if temperatures spike.  
*   **Week 4 (Security & Cloud):** Secure MQTT with TLS. Register one node to AWS IoT Core (Free Tier).  
  
**Guidance & Resources:**  
*   📘 **MQTT Theory:** [HiveMQ MQTT Essentials (Parts 1-10)](https://www.hivemq.com/mqtt-essentials/)  
*   🔧 **Broker Setup:** [Mosquitto Download](https://mosquitto.org/download/) | [Setup Video](https://www.youtube.com/watch?v=DH-VSS_4tGQ)  
*   📊 **Dashboard:** [Grafana + InfluxDB + MQTT Tutorial](https://www.youtube.com/watch?v=_DO2wHI6JWQ)  
*   ☁️ **AWS Cloud:** [AWS IoT Core Getting Started](https://docs.aws.amazon.com/iot/latest/developerguide/iot-gs.html)  
  
---  
  
# 🟠 PHASE 2: "THE SECURITY SPECIALIST" (Months 4-6)  
**Goal:** Cybersecurity foundations + Secure Hardware Project + Certifications.  
  
## 🛒 Phase 2 Hardware & Components Needed:  
*   **Access Control Parts:** RFID RC522 module, 4x4 Keypad, OLED display 0.96", Relay module, Solenoid Lock.  
*   **Software Tools:** Wireshark, TryHackMe account.  
  
---  
  
## 📅 MONTH 4: CYBERSECURITY DEEP DIVE  
  
### Week 1-4 Tasks:  
*   Learn TCP/IP, ARP, DNS, DHCP. Use Wireshark to capture your IoT system's network traffic.  
*   Study OWASP IoT Top 10 vulnerabilities.  
*   Implement AES-128/256 encryption on your ESP32.  
*   Begin CompTIA Security+ study (1-2 hours daily).  
  
**Guidance & Resources:**  
*   🎓 **Security+:** [Professor Messer SY0-701 Video Course (Free)](https://www.professormesser.com/security-plus/sy0-701/sy0-701-video/sy0-701-comptia-security-plus-course/)  
*   💻 **Labs:** [TryHackMe Pre-Security Path](https://tryhackme.com/path/outline/presecurity)  
*   🔧 **Network Analysis:** [Wireshark Download](https://www.wireshark.org/download.html)  
  
---  
  
## 📅 MONTH 5: FLAGSHIP PROJECT 3 - SECURE IoT ACCESS SYSTEM  
**Project Goal:** Enterprise-grade RFID + PIN access system with encryption.  
  
### Week 1-4 Tasks:  
*   **Week 1 (Hardware):** Wire ESP32 + RFID RC522 + Keypad + OLED + Relay.  
*   **Week 2 (Auth):** Encrypt RFID UIDs using AES before storing. Implement 2-Factor (Card + PIN).  
*   **Week 3 (Cloud):** Send access logs via MQTT (TLS) to Firebase. Build an admin dashboard in Node-RED.  
*   **Week 4 (Testing):** Implement brute-force protection (lockout). Write a Penetration Testing Report on your own system.  
  
**Guidance & Resources:**  
*   🔧 **RFID setup:** [ESP32 RFID Guide](https://randomnerdtutorials.com/esp32-rfid-rc522-arduino-ide/)  
*   🛡️ **Encryption Code:** [AES on ESP32 Library](https://github.com/suculent/thinx-aes-lib)  
*   ☁️ **Database:** [Firebase Realtime Database + ESP32](https://randomnerdtutorials.com/esp32-firebase-realtime-database/)  
  
---  
  
## 📅 MONTH 6: CERTIFICATIONS & PCB DESIGN  
  
### Week 1-4 Tasks:  
*   **Week 1-2:** Take practice exams and pass the CompTIA Security+ Exam.  
*   **Week 3 (KiCad):** Learn schematic capture. Design a custom PCB for your Phase 1 Sensor Node. Generate Gerber files.  
*   **Week 4:** Start AWS Cloud Practitioner study. Polish GitHub readmes.  
  
**Guidance & Resources:**  
*   💻 **PCB Software:** [KiCad Download](https://www.kicad.org/download/)  
*   📺 **PCB Tutorial:** [KiCad 7.0 Masterclass Series](https://www.youtube.com/playlist?list=PL3bNyZYHcRSUhUXUt51W6nKvxx2ORvUQB)  
*   🎓 **Cert Prep:** [AWS Cloud Quest (Free Badge)](https://explore.skillbuilder.aws/learn/course/external/view/elearning/11458/aws-cloud-quest-cloud-practitioner)  
  
---  
  
# 🟢 PHASE 3: "THE EDGE MASTER" (Months 7-9)  
**Goal:** Edge AI / TinyML deployment + ROS2 + Portfolio Polish.  
  
## 🛒 Phase 3 Hardware Needed:  
*   **AI Sensors:** I2S Microphone module (INMP441) or standard analog mic.  
*   **Platform:** Edge Impulse (Free Tier Account).  
  
---  
  
## 📅 MONTH 7: EDGE AI & TinyML  
  
### Week 1-4 Tasks:  
*   **Week 1-2:** Learn TensorFlow Lite Micro. Train a simple motion detection model on Edge Impulse using MPU6050 data.  
*   **Week 3-4 (Project 4):** Build the **Predictive Maintenance System**. Mount MPU6050 to a fan/motor. Record "Normal" and "Abnormal" vibrations. Train an anomaly detection model. Run inference directly on the ESP32 and publish warnings via MQTT.  
  
**Guidance & Resources:**  
*   🎓 **Course:** [HarvardX TinyML Professional Certificate (Free to Audit)](https://www.edx.org/professional-certificate/harvardx-tiny-machine-learning)  
*   🧠 **Platform:** [Edge Impulse Studio](https://studio.edgeimpulse.com/signup)  
*   📺 **Tutorial:** [Continuous Motion Recognition](https://www.youtube.com/watch?v=h3vGFpFEQIw)  
  
---  
  
## 📅 MONTH 8: ADVANCED SKILLS & ROS2  
  
### Week 1-4 Tasks:  
*   **Week 1:** Install Ubuntu (VM or dual-boot). Install ROS2 Humble. Run Turtlesim tutorials.  
*   **Week 2:** Connect your ESP32 to ROS2 via micro-ROS. Publish sensor data to ROS2 topics.  
*   **Week 3:** Deep dive into raw communication protocols (SPI, I2C, UART) at the register level.  
*   **Week 4:** System Design practice. Learn Git Flow and GitHub Actions (CI/CD).  
  
**Guidance & Resources:**  
*   💻 **ROS Platform:** [The Construct (Free ROS Courses)](https://www.theconstructsim.com/)  
*   📺 **ROS2 Videos:** [Articulated Robotics ROS2 Playlist](https://www.youtube.com/playlist?list=PLunhqkrRNRhYAffV8JDiFOatQXuU-NnxT)  
*   🔧 **micro-ROS:** [FreeRTOS + micro-ROS integration](https://micro.ros.org/docs/tutorials/core/first_application_rtos/freertos/)  
  
---  
  
## 📅 MONTH 9: JOB-READY EXECUTION  
  
### Week 1-4 Tasks:  
*   **Week 1:** Complete HarvardX TinyML and get your (financial aid) certificate. Complete Cisco Networking Academy free certs (IoT Fundamentals).  
*   **Week 2 (Resume):** Structure your CV highlighting: FreeRTOS, MQTT, PID, TLS, Edge AI, and ROS2. List all 4 flagship projects.  
*   **Week 3 (Interview Prep):** Practice explaining RTOS concepts, Memory limits, Interrupts, and System Architecture on a whiteboard.  
*   **Week 4 (Apply):** Research 50 companies. Tailor resumes. Network actively on LinkedIn. Include links to your GitHub and YouTube demo videos.  
  
**Guidance & Resources:**  
*   📝 **GitHub Profile:** [Awesome GitHub Profile README Templates](https://github.com/abhisheknaiidu/awesome-github-profile-readme)  
*   🎓 **Final Free Certs:** [Cisco NetAcad Courses](https://www.netacad.com/) (Introduction to Cybersecurity, IoT Fundamentals).  
  
---  
  
# 🕒 DAILY EXECUTION TRACKER TEMPLATE  
*Build this in Notion or Excel.*  
  
| Time Block | Focus Area | Activity Example |  
| :--- | :--- | :--- |  
| **Morning (1.5 hrs)** | Theory & Learning | Watch Brian Douglas PID videos / Take Notes |  
| **Afternoon (2-3 hrs)** | Hands-On Building | Wire ESP32, write C++ code, debug compiler errors |  
| **Evening (1 hr)** | Documentation | Push code to GitHub, write README, post on LinkedIn |  
  
**The Golden Rules:**  
1. **BUILD > LEARN:** Spend 70% of your time writing code and wiring circuits, 30% watching tutorials.  
2. **DOCUMENT EVERYTHING:** A project without a GitHub README and a Video Demo doesn't exist to an employer.  
3. **DEBUGGING IS WORKING:** Getting stuck for 3 hours on an I2C bug *is* the actual job. Embrace it.