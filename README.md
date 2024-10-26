# Reflective IR Sensor Alarm System with 555 Timer

This project is a simple IR-based sensor system that uses a reflective IR sensor setup and a 555 timer IC in monostable mode. When a person or object reflects the IR light back to the IR photodiode, it triggers the 555 timer, activating an active buzzer for approximately 5 seconds. This can be adapted for applications like an automatic doorbell, person detection alarm, and more.

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Applications](#applications)
4. [Project Files](#project-files)
5. [Hardware Setup](#hardware-setup)
6. [Getting Started](#getting-started)
7. [License](#license)

## Overview

- **IR LED and Photodiode**: The IR LED emits infrared light, which is detected by the photodiode when an object reflects the light. A heat shrink cover is recommended for the IR LED and photodiode to prevent interference from surrounding light.
- **555 Timer IC**: Configured in monostable mode, the 555 IC is triggered by the IR photodiode’s output signal. When triggered, it activates the output (an active buzzer) for a set duration (approximately 5 seconds).
- **Output (Active Buzzer)**: Produces sound when the 555 IC output is high, which can be used for alarms or notifications.

### Features
- **Reflective IR Detection**: The adjacent IR LED and photodiode are covered with heat shrink to improve directional sensitivity.
- **Monostable Timer**: Provides a fixed 5-second output signal on detection.
- **Adaptable Output**: Can be connected to various output devices, like a buzzer or LED.

## Applications
1. **Automatic Doorbell**: Detects a person at the entrance and sounds a doorbell.
2. **Entry Alert**: Notifies staff when someone enters a room or area.
3. **Automatic Lighting**: Turns on lights when someone enters a hallway or room.
4. **Obstacle Detection**: Used in robotics to detect nearby obstacles.
5. **Home Security Alarm**: Sounds an alarm when someone is near a monitored area.
6. **Vehicle Reversing Aid**: Alerts the driver if an obstacle is detected while reversing.

## Project Files
- **KiCad_Project/**: Contains all the KiCad files:
  - `.pro`: Project file.
  - `.sch`: Schematic file showing the 555 timer in monostable configuration with IR LED and photodiode.
  - `.kicad_pcb`: PCB layout for assembling the components.
  - `libraries/` and `footprints/`: Any custom library or footprint files.
- **Gerber/**: Gerber files for PCB manufacturing.
- **Images/**: Screenshots of the schematic and PCB layout.

## Hardware Setup
- **IR LED and IR Photodiode**: Positioned adjacent to each other and enclosed in heat shrink tubing to minimize interference and enhance detection accuracy. Place the setup in a location where it can detect reflections from objects or people passing by.
- **555 Timer**: Connected in monostable mode. The output pulse length can be adjusted by changing the timing resistor and capacitor.
- **Active Buzzer**: Connected to the output of the 555 timer to sound an alert for a 5-second duration upon detection.

### Circuit Schematic and PCB Layout
![Schematic](Images/schematic.png)
![PCB Layout](Images/pcb_layout.png)

## Getting Started
1. **Download** the repository files.
2. Open the project files in KiCad for viewing or modification.
3. **Assemble the components** as per the schematic, ensuring the IR LED and photodiode are correctly positioned with heat shrink to isolate their light.
4. **Test the circuit** by placing objects or people near the sensor and observing the 5-second buzzer response.

## License
This project is open-source and available under the MIT License. Please refer to the `LICENSE` file for more details.
