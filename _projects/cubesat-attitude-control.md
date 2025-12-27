---
title: "CubeSat Attitude Control Using Reaction Wheels"
collection: projects
permalink: /projects/cubesat-attitude-control/
excerpt: "Design and implementation of a CubeSat command and data handling system with reaction-wheel-based attitude control."
github_url: "https://github.com/juanj-mg/"
share: false
comments: false
---


## Quick links

- **Code & files (GitHub repo):** [{{ page.github_url }}]({{ page.github_url }})

## Overview

This project was developed as a **final project for graduate-level Aerospace Control Systems and Aerospace Systems courses**.  
The objective was to design and implement a **CubeSat command and data handling (C&DH) architecture** capable of stabilizing and controlling spacecraft attitude using **reaction wheels**.

The project emphasizes **control theory implementation, embedded systems, and aerospace systems integration**, rather than theoretical research.

---

## System Description

The CubeSat control system consists of the following components:

- Embedded microcontroller-based command and data handling (C&DH)
- Inertial Measurement Unit (IMU) for attitude sensing
- Reaction wheels for attitude actuation
- Real-time attitude estimation and control logic
- Web-based interface for commanding and monitoring system behavior

The system was designed to operate in real time, receiving commands, estimating spacecraft attitude, and generating control torques to regulate orientation.

---

## Control Approach

The control architecture includes:

- Attitude estimation using inertial sensor data
- Feedback control laws for reaction wheel torque commands
- Conversion of desired body torques into reaction wheel actuation
- Closed-loop stabilization of spacecraft orientation

The control logic was implemented directly on the embedded platform, emphasizing practical considerations such as timing, sensor noise, and actuator limitations.

---

## Software and Tools

- **Embedded development:** ESP32 microcontroller
- **Programming languages:** C/C++, JavaScript, HTML, CSS
- **Control implementation:** Real-time embedded control loops
- **Interface:** Web-based command and visualization dashboard

---

## Educational Context

This project served as a **capstone-style final project**, integrating concepts from:

- Aerospace control systems
- Spacecraft dynamics and attitude control
- Embedded systems and real-time computing
- Aerospace systems engineering

---

## Notes

This project is presented as an **academic engineering course project** and is not intended as a research contribution or publication.
