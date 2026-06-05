# Keyboard Key Detection

ROS2 node for detecting and publishing keyboard key events. Maps physical key presses to ROS2 topics for use in teleoperation and human-robot interaction pipelines.

## Overview

Captures keyboard input in a ROS2 node and publishes key events as messages. Useful as a base for custom keyboard-driven robot control beyond the standard `teleop_twist_keyboard`.

## Stack

- **ROS2 Humble**
- **Python** — `pynput` / `keyboard` library for key capture
- **std_msgs / custom msg** — key event publishing

## Usage

```bash
colcon build
source install/setup.bash

ros2 run keyboard_detection key_detector
```

Subscribe to `/key_event` to receive key press/release events in other nodes.

## Robotronics Club — IIT Mandi

Part of the Robotronics Club recruitment task series (Task 5.1).

## Author

Rohit Jangra · [github.com/Rohitjangra7370](https://github.com/Rohitjangra7370)
