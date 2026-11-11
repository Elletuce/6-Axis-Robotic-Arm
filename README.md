# 6-DOF Robotic Arm

A custom-designed, 6-degree-of-freedom robotic arm developed as a personal engineering project. This repository contains the mechanical CAD designs, electronic hardware documentation, and software used to control the robotic arm.

The goal of this project is to design, manufacture, and program a functional robotic arm capable of precise movement and object manipulation.

## Project Overview

The robotic arm is designed and built from the ground up, incorporating custom mechanical components, stepper motor actuation, and microcontroller-based control.

Key objectives include:
- Designing and manufacturing a custom robotic arm.
- Developing a multi-axis motion control system.
- Implementing inverse kinematics for positioning the end effector.
- Integrating stepper motors and motor drivers.
- Developing communication between a PC and an ESP32 microcontroller.
- Exploring AI-assisted control and automated movement.

## Mechanical Design

The mechanical components are designed using **SolidWorks**. The CAD files include the individual components, subassemblies, and complete robotic arm assembly.

Mechanical design considerations include:
- Structural rigidity and load capacity.
- Weight reduction and material selection.
- Custom gearbox and transmission designs.
- Motor mounting and joint integration.
- Cable routing and electronic component placement.

## Hardware

| Component | Description |
|---|---|
| Microcontroller | ESP32 |
| Shoulder Motor | NEMA 23 Stepper Motor |
| Other Joint Motors | NEMA 17 Stepper Motors |
| Motor Driver | DM542 |
| Motor Drivers | TMC2209 |
| Power Supply | 24V DC |
| Frame | Custom-designed components |

*Hardware specifications are subject to change as development progresses.*

## Software

The control system uses Python for high-level control and an ESP32 for low-level motor control.

**Python (PC)**
- High-level robotic arm control.
- Inverse kinematics calculations.
- Joint position calculations.
- Communication with the ESP32.
- Future AI-assisted control integration.

**ESP32 (Microcontroller)**
- Receives movement commands from the PC.
- Generates step and direction signals.
- Controls individual stepper motor drivers.
- Coordinates joint movement.

## Repository Structure

```text
Robotic-Arm/
│
├── CAD/
│   ├── Parts/
│   ├── Assemblies/
│   └── Drawings/
│
├── Software/
│   ├── Python/
│   │   ├── inverse_kinematics.py
│   │   ├── motion_control.py
│   │   └── communication.py
│   │
│   └── ESP32/
│       ├── main.cpp
│       └── motor_control.cpp
│
├── Electronics/
│   ├── PCB/
│   ├── Schematics/
│   └── Wiring/
│
├── Documentation/
│   ├── Images/
│   └── Specifications/
│
└── README.md
```

## Development Status

- [x] Initial mechanical design and CAD development
- [x] Stepper motor and driver selection
- [x] ESP32 hardware integration
- [x] Initial PC-to-ESP32 communication
- [ ] Complete mechanical assembly
- [ ] Complete motor integration
- [ ] Implement inverse kinematics
- [ ] Implement coordinated joint movement
- [ ] Implement position feedback and calibration
- [ ] Integrate AI-assisted control
- [ ] Complete robotic arm testing

## Future Improvements

- Closed-loop position control using rotary encoders.
- Improved motion planning and trajectory generation.
- Dynamic load compensation.
- AI-assisted natural language movement commands.
- Improved repeatability and positioning accuracy.

## License

License and usage terms to be determined.

---

**Project Status:** In Development
