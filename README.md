# GrowBot – Autonomous Fertilizer Delivery Robot

## Overview
This repository documents the design and development of GrowBot, an autonomous, tow-behind fertilizer delivery system built on the ELEGOO Smart Robot Car platform. The system was engineered to autonomously navigate a predefined course, avoid obstacles, and selectively dispense simulated fertilizer (pom-poms) at designated locations.

The project integrates mechanical design, embedded systems, sensing, and autonomous control, and was developed as a team-based engineering design project following a formal proposal and testing process.

---

## System Capabilities
GrowBot was engineered to perform the following tasks autonomously:
- **Line-following navigation** using line tracking and infrared sensors
- **Obstacle detection and avoidance** using ultrasonic distance sensors
- **Targeted fertilizer delivery** via a motorized spinning-wheel dispensing mechanism
- **Tow-behind operation**, fully powered and controlled by the ELEGOO Smart Robot Car

All functions were executed without manual intervention during operation.

---

## Mechanical Design

### Trailer and Dispensing Mechanism
- A custom tow-behind trailer was designed to attach non-destructively to the robot car
- The fertilizer dispenser uses a gravity-fed vertical tube combined with a servo-driven mechanical arm
- A clog-resistant design ensures consistent release of fertilizer units
- Components were optimized for low weight to avoid overloading the robot

### CAD Design and Fabrication
- AutoCAD was used to create detailed technical drawings (top, front, and side views) following third-angle projection standards
- SketchUp was used during early-stage concept modeling and layout
- Key components were 3D printed using PLA filament
- Multiple design iterations were required to refine fit, alignment, and dispensing reliability

#### AutoCAD Sketches
![CAD Sketch](./_Figures/cad_sketch.png)
These drawings document the final dimensions, servo placement, and dispensing geometry used for fabrication and assembly.

---

## Electronics and Control System
- **Microcontroller:** Arduino (ELEGOO Smart Robot Car)
- **Sensors:**
  - Line tracking sensors for path following
  - Infrared sensor for navigation support
  - Ultrasonic sensor (HC-SR04) for obstacle detection
- **Actuators:**
  - DC motors for vehicle motion
  - Servo motor (SG90) for fertilizer dispensing

Custom Arduino code was developed to coordinate sensor inputs with motor outputs, enabling autonomous navigation, obstacle avoidance, and controlled dispensing.

---

## Autonomous Behavior
- The robot follows a predefined path using a line-following algorithm
- Ultrasonic sensing detects obstacles and triggers avoidance maneuvers
- Fertilizer is dispensed gradually and only at required locations
- Upon task completion, the robot aligns with the exit zone and signals completion

---

## Testing and Performance
- Tested on a **custom obstacle course**
- Completed the course in **32 seconds**
- Achieved 100% accuracy in obstacle avoidance and fertilizer delivery
- Consistently dispensed all five fertilizer units without clogging
- Total system cost: $98.03 CAD 

---

## Results and Limitations
### Strengths
- Reliable autonomous navigation
- Accurate and controlled fertilizer dispensing
- Lightweight, low-cost design
- Non-destructive attachment to the robot platform

### Limitations
- Servo motor power consumption reduced battery endurance
- Wheelbase limited maneuverability in sharp turns
- Future improvements could include power optimization and enhanced mobility

---

## Final Product
![Final Design](./_Figures/final_design.png)

![Servo-Controlled Dispensing Arm](./_Figures/servo_dispensing_arm.jpg)

The final prototype demonstrates a fully integrated autonomous agricultural delivery system.

---

## Team Experience and Learning Outcomes
This project enabled the team to:
- Collaborate on a complete engineering system from concept to prototype
- Apply CAD, 3D printing, and mechanical fabrication techniques
- Write and debug Arduino code for autonomous robotic behavior
- Adapt designs through testing, iteration, and constraint management

---

## Author
Masa Damdoum  
Electrical Engineering (Co-op)  
University of Windsor


---

## Disclaimer
GrowBot is a prototype developed for academic and demonstration purposes only and is not intended for real-world agricultural deployment.
