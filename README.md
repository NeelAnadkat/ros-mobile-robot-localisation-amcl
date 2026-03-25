# ros-mobile-robot-localisation-amcl
Autonomous mobile robot localisation in a known environment using ROS Noetic, TurtleBot3, and Adaptive Monte Carlo Localisation (AMCL)
# Mobile Robot Localisation using AMCL & ROS

## 🤖 Project Overview
This project implements **Adaptive Monte Carlo Localisation (AMCL)** for a mobile robot within a known environment. Using the **ROS Noetic** framework and **TurtleBot3** simulation, the system estimates the robot's pose by matching laser scan data against a pre-existing occupancy grid map.

## 🛠️ Tech Stack
- **Framework:** ROS Noetic (Robot Operating System)
- **Simulator:** Gazebo & RViz
- **Robot:** TurtleBot3 (Burger)
- **Algorithms:** Particle Filter (AMCL), Odometry-based Motion Model

## 🚀 Key Features
- **Probabilistic Localisation:** Utilized a particle filter to represent the probability distribution of the robot's pose.
- **Sensor Fusion:** Integrated data from `/scan` (Lidar), `/odom` (Odometry), and `/map` topics.
- **Real-time Visualization:** Monitored the convergence of the particle cloud in RViz during teleoperation.
- **Accuracy:** Successfully demonstrated that the particle cloud concentrates around the actual robot position as sensor data increases over time.
