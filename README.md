# LiDAR-Based Autonomous Obstacle Avoidance Rover

This repository contains the Python code and control logic for an autonomous rover designed for obstacle avoidance in real-time using a low-cost LiDAR sensor and a Raspberry Pi. The project aims to address the unique challenges of Indian road conditions, such as unstructured traffic, unpredictable pedestrian behavior, and poor lane discipline, without relying on high-end deep learning architectures or expensive sensor suites.

## 🚗 Project Overview

- **Platform**: Raspberry Pi (tested with Pi 3/4)
- **Primary Sensor**: YDLiDAR X4 Pro
- **Control Logic**: Rule-based obstacle avoidance
- **Key Features**:
  - Real-time LiDAR data processing
  - Dynamic decision-making for turns and stops
  - Emergency collision detection and braking
  - Sector-based distance filtering (front, side, rear)
  - Lightweight, affordable hardware setup

## 📁 Files Included

| File Name                  | Description                                           |
|---------------------------|-------------------------------------------------------|
| `Appendix_A_Rover_Code.txt` | Main Python code used on the rover                   |
| `README.md`               | This file, containing an overview and instructions    |

## ⚙️ System Requirements

- Raspberry Pi 3 or higher
- Python 3.6+
- `pigpio`, `numpy`, `pyserial`, `RPi.GPIO`
- YDLiDAR X4 Pro (or similar LiDAR with serial interface)

## 🧠 Methodology

Unlike AI-driven AVs, this prototype uses:
- **Rule-based logic** for decision-making
- **Zonal distance thresholds** (front, left, right, rear)
- **Servo steering and throttle control** through PWM
- **Threaded LiDAR data handling** for real-time updates

## 🧪 Real-World Performance

The rover was tested across various obstacle scenarios and demonstrated:
- Timely reaction to near-field hazards
- Capability to navigate constrained paths
- Stable maneuvering under tight steering conditions

## 🔬 Academic Context

This code was developed as part of a research prototype exploring low-cost autonomy for Indian road infrastructure. It is accompanied by a research paper that investigates latency, decision logic, and performance metrics on urban-like unstructured paths.

## 📚 Citation

If you use this code in your research or publication, please cite the following:

