# Straight-Line-Motion-Bot

This project is a precision-controlled Arduino-based robot designed to move in a perfectly straight line, minimizing drift or deviation during motion. It leverages real-time feedback from encoder motors to dynamically adjust wheel speeds and maintain a straight trajectory, even on uneven surfaces or when motors differ slightly in performance.

The robot is powered by an Arduino Nano, which serves as the brain of the system. It uses two encoder-equipped DC motors for propulsion, allowing the bot to measure actual wheel rotations in real time. This data is then used to ensure that both wheels rotate at synchronized speeds, effectively correcting any deviation from a straight path.

A push button is integrated to act as the start/stop trigger for the bot. When pressed, the bot begins its forward movement and automatically monitors its heading using encoder feedback. If either motor begins to rotate faster or slower than intended, the Arduino compensates by adjusting the PWM signals sent to the motors. This simple yet effective closed-loop control strategy allows the bot to stay on course with impressive accuracy.

To enhance usability, two LEDs are used as visual indicators. One LED is powered on and ready, while the other indicates when the bot is actively moving. These visual cues help users quickly understand the current state of the robot at a glance.

The core objective of this bot is to demonstrate straight-line motion correction using encoder feedback without relying on complex navigation systems or external sensors like gyroscopes or compasses. It’s an excellent example of how fundamental principles of control systems and feedback loops can be applied in embedded systems and robotics.

Whether you're a student learning about robotics and feedback control, or a hobbyist looking to build precise, reliable motion systems, this project provides a practical and educational foundation. It's a great entry point into topics like PID control, encoder-based navigation, and real-world robotics challenges such as mechanical drift and motor mismatch.

# 🔧 Key Components:
Arduino Nano: Central microcontroller for logic and control.

2x N20 Encoder Motors: Provide rotational feedback for closed-loop control.

2x LEDs: Indicate power status and movement state.

Push Button: User input to initiate motion.

Motor Driver: (TB6612FNG) Controls the speed and direction of motors via PWM.

This repository contains all the necessary code, wiring diagrams, and setup instructions to replicate the build. Contributions and improvements are welcome, especially enhancements such as implementing PID control for even finer trajectory correction.
