# Simple Rover ROS2

A simple two-wheel differential drive rover robot designed using ROS 2 framework.

## Features

- Differential drive mobile robot
- URDF/Xacro robot description
- RViz visualization
- ROS 2 compatible package structure

## Package Structure

```text
my_rover_description/
├── urdf/
├── launch/
├── rviz/
├── meshes/
├── package.xml
├── CMakeLists.txt
└── README.md
```

## Requirements

- ROS 2
- xacro
- robot_state_publisher
- joint_state_publisher_gui
- rviz2

## Run Robot Description

```bash
ros2 launch my_rover_description display.launch.py
```

## Visualize in RViz

```bash
ros2 run rviz2 rviz2
```

## Robot Frames

```text
base_footprint
    |
base_link
   / \
left_wheel_link
right_wheel_link
```

## Author

Rahul Singh
