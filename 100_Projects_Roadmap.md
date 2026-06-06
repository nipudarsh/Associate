# 🚀 THE 100 PROJECT GAUNTLET
## From Bare Metal Basics to Advanced Cyber-Physical Systems

This is a complete, progressive list of 100 projects designed to take you from a complete beginner to a highly advanced Embedded, IoT, and Robotics Engineer. They follow the skills outlined in your 9-Month Roadmap.

---

### 🟢 LEVEL 1: BARE METAL & HARDWARE FUNDAMENTALS (Projects 1-20)
*Goal: Understand GPIO, basic sensors, interrupts, and simple logic without any OS.*

1. **Hello World Blink:** Blink an LED, then modify it to blink without using `delay()` (using `millis()`).
2. **Traffic Light Controller:** 3 LEDs with a state machine for timing and a pedestrian crossing button.
3. **Hardware Debouncer:** Count button presses accurately using hardware debouncing (capacitors/resistors).
4. **Software Debouncer:** Count button presses using purely software debounce logic.
5. **RGB Color Mixer:** Use 3 potentiometers to read analog values (ADC) and control an RGB LED via PWM.
6. **Night Light:** Use an LDR (photoresistor) to automatically turn on an LED when the room goes dark.
7. **Ultrasonic Ruler:** Read an HC-SR04 sensor and print the distance to the Serial Monitor.
8. **Parking Assistant:** Ultrasonic sensor + Buzzer. The buzzer beeps faster as an object gets closer.
9. **Digital Thermometer:** Read a DHT11/DHT22 and display the temperature on an I2C 16x2 LCD.
10. **Servo Sweeper:** Smoothly sweep a servo motor 180 degrees using PWM loops.
11. **Analog Dial:** Control the exact angle of a servo motor using a potentiometer.
12. **Stopwatch:** Use hardware timer interrupts to build a precise stopwatch on a 4-digit 7-segment display.
13. **Security Keypad:** Read a 4x4 matrix keypad and print pressed keys to the serial monitor.
14. **Simple Door Lock:** Combine the keypad and a servo. Enter "1234" to rotate the servo (unlock).
15. **RFID UID Reader:** Connect an RC522 RFID reader via SPI and print the unique ID of scanned cards.
16. **RPM Counter:** Use a Hall Effect sensor and hardware interrupts to calculate the RPM of a spinning magnet.
17. **Sound Level Meter:** Read an analog microphone, calculate the peak-to-peak amplitude, and display a bar graph on the Serial Plotter.
18. **IR Remote Relay:** Decode signals from a TV remote (IR receiver) to toggle a high-voltage relay.
19. **EEPROM Memory Logger:** Save the number of system reboots permanently into the microcontroller's EEPROM/Flash.
20. **Classic Bluetooth Chat:** Use ESP32 Bluetooth Classic to send and receive text messages to a smartphone app.

---

### 🟡 LEVEL 2: IOT, NETWORKING & PROTOCOLS (Projects 21-40)
*Goal: Connect to the internet, handle APIs, basic MQTT, and understand web servers.*

21. **Wi-Fi Scanner:** Scan for nearby Wi-Fi networks and print their SSID and signal strength (RSSI).
22. **Captive Portal:** Create an Access Point (AP) that serves a web page to input Wi-Fi credentials for setup.
23. **Local Web Server:** Host an HTML/CSS page on the ESP32 to toggle an LED from a PC browser.
24. **Web Dashboard:** Host a webpage featuring live-updating gauges showing DHT22 temperature data.
25. **Internet Clock (NTP):** Fetch the exact time from a Network Time Protocol server and display it on an OLED.
26. **Weather API Fetcher:** Connect to the OpenWeatherMap API, parse the JSON response, and display the weather.
27. **Basic MQTT Publisher:** Connect to a public broker (like HiveMQ) and publish temperature every 5 seconds.
28. **Basic MQTT Subscriber:** Subscribe to an MQTT topic to remotely toggle a relay from anywhere in the world.
29. **ThingSpeak Logger:** Push environmental data to ThingSpeak and view the auto-generated cloud graphs.
30. **Discord Webhook Alert:** Send an automated message to a Discord server when a PIR motion sensor is triggered.
31. **Email Intruder Alert:** Send an email with a timestamp when a door is opened (magnetic reed switch).
32. **Telegram Bot Controller:** Build a Telegram bot hosted on the ESP32 to reply to text commands (e.g., "/status").
33. **Firebase Realtime Database:** Log RFID card scans directly into Google Firebase for cloud storage.
34. **BLE Beacon Scanner:** Scan for Bluetooth Low Energy (BLE) MAC addresses and estimate their distance.
35. **BLE Custom Service:** Create a BLE GATT server on the ESP32 to broadcast battery level to a phone.
36. **Over-The-Air (OTA) Updates:** Update the ESP32's firmware via Wi-Fi without using a USB cable.
37. **I2C Scanner Utility:** Write a script to scan the I2C bus and report the hex addresses of all connected devices.
38. **SPI Flash Reader:** Interface with an external SPI Flash memory chip to read/write raw bytes.
39. **UART Bridge:** Establish two-way serial communication between an ESP32 and an Arduino Uno.
40. **Modbus RTU Master:** Read holding registers from a simulated industrial Modbus slave device over RS485.

---

### 🟠 LEVEL 3: FREERTOS, PID & KINEMATICS (Projects 41-60)
*Goal: Multitasking, deterministic timing, closed-loop control, and smooth physical motion.*

41. **FreeRTOS Multi-Blink:** Create 3 independent FreeRTOS tasks blinking LEDs at completely different rates.
42. **Task Suspension:** Create a task that suspends another task when a button is pressed, and resumes it on a second press.
43. **FreeRTOS Queues:** Task 1 reads an ADC; Task 2 processes the data; pass the data safely using a Queue.
44. **Mutex Protected I2C:** Use a Mutex semaphore to prevent two FreeRTOS tasks from crashing the I2C bus while reading the same sensor.
45. **Software Timers:** Use FreeRTOS software timers to build an auto-sleep watchdog feature.
46. **Binary Semaphore Interrupt:** Trigger a hardware interrupt (button), which gives a semaphore to unblock a high-priority processing task.
47. **Encoder Speed Calculator:** Read an encoder using hardware interrupts and calculate exact RPM every 100ms.
48. **Open-Loop Motor Mapping:** Map PWM values (0-255) to actual motor RPM and graph the non-linear relationship.
49. **PID Speed Controller:** Implement a PID loop to keep a DC motor at an exact RPM regardless of physical load/friction.
50. **PID Line Follower:** Build a robot that uses a PID algorithm to smoothly follow a line (no jerky left/right movements).
51. **IMU Complementary Filter:** Combine MPU6050 accelerometer and gyroscope data to get a stable, drift-free tilt angle.
52. **Self-Balancing 1D Beam:** Balance a ping-pong ball on a servo-controlled beam using ultrasonic distance and PID.
53. **Cruise Control Robot:** A differential drive robot that maintains a constant forward speed up and down inclines.
54. **Stepper Motor Acceleration:** Control a NEMA 17 stepper motor with smooth trapezoidal acceleration/deceleration curves.
55. **Smart Blinds State Machine:** FreeRTOS system: Task 1 checks light, Task 2 checks time, Task 3 drives stepper, Task 4 handles MQTT overrides.
56. **Load Cell Digital Scale:** Interface an HX711 with a load cell, applying rolling average filters to get sub-gram precision.
57. **Sensor Fusion Compass:** Combine an MPU6050 with a Magnetometer (HMC5883L) to create a tilt-compensated compass.
58. **Differential Drive Kinematics:** Convert desired Robot Velocity (V, Omega) into Left and Right wheel RPM targets.
59. **Robot Odometry:** Calculate the robot's X,Y position in a room based purely on wheel encoder ticks over time.
60. **PID Heating Element:** Control a heating pad with PWM and a thermistor to maintain water at exactly 40.0°C.

---

### 🔴 LEVEL 4: CYBERSECURITY & EDGE AI (TINYML) (Projects 61-80)
*Goal: Secure systems against attacks, and run machine learning models on microcontrollers.*

61. **TLS/SSL MQTT:** Upgrade your MQTT connection to use TLS 1.2 encryption and verify server certificates.
62. **AES-256 Payload Encryption:** Encrypt a sensor payload using AES before sending it over Wi-Fi/Bluetooth.
63. **SHA-256 Hashing:** Hash an RFID UID with a salt so the true UID is never stored in memory.
64. **JWT Authentication:** Generate and verify JSON Web Tokens (JWT) for secure REST API access on the ESP32.
65. **Brute Force Defense:** Lockout the keypad for 5 minutes after 3 incorrect PIN attempts, storing state in EEPROM.
66. **Wi-Fi Deauth Detector:** Put the ESP32 in promiscuous mode to detect and alert on Wi-Fi deauthentication attacks.
67. **Hardware Random Number Generator:** Utilize the ESP32's internal noise generator to create cryptographically secure keys.
68. **Offline-First Cache:** IoT system that logs data to an SD card if Wi-Fi goes down, and bulk-uploads when reconnected.
69. **Intrusion Detection System (IDS):** Monitor login times. If a login occurs at 3 AM, trigger a silent cloud alarm.
70. **Secure OTA Updates:** Implement OTA updates that verify a digital signature before applying the new firmware.
71. **Edge Impulse Hello World:** Collect accelerometer data, upload to Edge Impulse, and train a basic "Idle vs. Shaking" model.
72. **Motion Classification (TinyML):** Train a model to distinguish between "Walking," "Running," and "Jumping" based on IMU data.
73. **Predictive Maintenance:** Mount an IMU on a fan. Train an anomaly detection model to flag when the fan is unbalanced or failing.
74. **Keyword Spotting:** Connect an I2S microphone and train a neural network to recognize the word "Activate."
75. **Glass Break Detector:** Use audio classification to detect the specific frequency profile of breaking glass.
76. **Snore Tracker:** Classify microphone data to detect and log the frequency of snoring during sleep.
77. **Posture Corrector Wearable:** A wearable IMU that uses TinyML to learn your specific "bad posture" and vibrates to correct you.
78. **ESP32-CAM Image Capture:** Set up an ESP32-CAM to take a photo and upload it to an FTP server when motion is detected.
79. **Basic Object Detection:** Train a tiny vision model to detect whether a person is in the frame of the ESP32-CAM.
80. **Smart Sorting Conveyor:** Use TinyML vision to identify "Defective" vs "Good" items and use a servo to sort them.

---

### ⚫ LEVEL 5: EXPERT SYSTEMS & ROS2 (Projects 81-100)
*Goal: Distributed systems, professional robotics frameworks, and industrial-grade architectures.*

81. **ESP-MESH Network:** Connect 5 ESP32s in a self-healing mesh network without relying on a central router.
82. **Mosquitto VPS Broker:** Deploy a Linux VPS (DigitalOcean/AWS), secure it, and host your own global MQTT broker.
83. **TIG Stack Dashboard:** Set up Telegraf, InfluxDB, and Grafana on a Raspberry Pi to visualize your complete network.
84. **Automated Factory Digital Twin:** Create a Grafana dashboard that visually mimics the state of 3 physical robot arms.
85. **micro-ROS Publisher:** Connect an ESP32 to a PC running ROS2 via micro-ROS and publish IMU data as a `sensor_msgs/Imu`.
86. **ROS2 Teleop Node:** Write a Python ROS2 node on your PC that subscribes to keyboard inputs and publishes `cmd_vel` to the ESP32.
87. **Robot URDF Modeling:** Write an XML (URDF) file describing your physical robot and visualize it in RViz2.
88. **TF2 Transform Broadcaster:** Publish the coordinate transformations between your robot's center, wheels, and sensors in ROS2.
89. **Gazebo Simulation:** Simulate your robot in Gazebo and drive it around a virtual world using ROS2.
90. **LIDAR Integration:** Connect an RPLidar A1 to ROS2 and visualize the 2D laser scan point cloud in RViz2.
91. **Basic SLAM:** Use `slam_toolbox` in ROS2 to drive your robot around a room and generate a 2D occupancy grid map.
92. **Nav2 Waypoint Navigation:** Use the ROS2 Nav2 stack to make the robot autonomously drive to a specific X,Y coordinate on your map.
93. **Obstacle Avoidance in Nav2:** Configure the local costmap so the robot actively paths around moving humans while navigating.
94. **Multi-Agent ROS2:** Simulate two different robots in ROS2 sharing the same map but avoiding each other.
95. **Industrial Modbus Bridge:** Build an ESP32 bridge that reads industrial Modbus RS485 sensors and translates them to ROS2 topics.
96. **AWS IoT Core Fleet Management:** Provision certificates for 3 "vehicles" (ESP32s), connect to AWS IoT, and use AWS Rules to filter data into DynamoDB.
97. **Voice-Commanded Robot:** Integrate Google Assistant with Node-RED to publish MQTT commands that trigger ROS2 navigation goals.
98. **Kalman Filter Sensor Fusion:** Implement an Extended Kalman Filter (EKF) in ROS2 to fuse wheel odometry with IMU data for perfect localization.
99. **Computer Vision Follower:** Use OpenCV on a Raspberry Pi/PC to track a colored ball, sending ROS2 velocity commands to the ESP32 to follow it.
100. **THE MASTERPIECE:** A fully autonomous robot featuring: FreeRTOS hardware management, PID motor control, Encrypted MQTT telemetry to AWS, micro-ROS integration, Nav2 autonomous LIDAR mapping, and Edge AI predictive maintenance on its own motors.

---
*Created as part of the Unified Execution Blueprint.*