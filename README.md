# Simple Rover ROS2 Project

A differential drive rover simulation built using ROS2, Gazebo, RViz, URDF/Xacro, and ros2_control.

## Features

* Differential drive robot
* Gazebo simulation
* RViz visualization
* ros2_control integration
* Controller configuration
* Custom URDF/Xacro robot description
* Launch files for simulation and visualization

---

# Project Structure

```bash
simple_rover/
├── src/
│   ├── my_rover_description/
│   └── my_rover_bringup/
├── .gitignore
└── README.md
```

---

# Requirements

* Ubuntu 24.04
* ROS2 Jazzy
* Gazebo Harmonic

---

# Install Dependencies

```bash
sudo apt update
sudo apt install ros-jazzy-desktop -y
sudo apt install ros-jazzy-gazebo-ros-pkgs -y
sudo apt install ros-jazzy-ros2-control ros-jazzy-ros2-controllers -y
```

---

# Build Workspace

```bash
cd ~/simple_rover
source /opt/ros/jazzy/setup.bash
colcon build
```

After build:

```bash
source install/setup.bash
```

---

# Run RViz Display

```bash
ros2 launch my_rover_description display.launch.py
```

---

# Run Gazebo Simulation

```bash
ros2 launch my_rover_description gazebo.launch.py
```

---

# Teleop Control

Open another terminal:

```bash
source ~/simple_rover/install/setup.bash
ros2 run teleop_twist_keyboard teleop_twist_keyboard
```

---

# Controllers

Controller configuration file:

```bash
my_rover_bringup/config/my_rover_controller.yaml
```

---

# Packages

## my_rover_description

Contains:

* URDF/Xacro files
* Meshes
* RViz configuration
* Gazebo launch files

## my_rover_bringup

Contains:

* ros2_control configuration
* Controller setup
* Bringup configuration

---

# Useful Commands

## Rebuild Workspace

```bash
colcon build --symlink-install
```

## Source Workspace

```bash
source install/setup.bash
```

## List ROS2 Nodes

```bash
ros2 node list
```

## List Topics

```bash
ros2 topic list
```

---

# GitHub

Repository:

[https://github.com/Rahul-singh-95/simple-rover-test](https://github.com/Rahul-singh-95/simple-rover-test)

---

# Author

Rahul Singh
