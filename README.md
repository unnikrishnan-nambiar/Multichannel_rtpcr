# 4-Channel Real-Time PCR Based on ARM Cortex

## Overview

This project implements a **4-channel real-time PCR** system utilizing **ARM Cortex-A72** and **ATmega2560** for DNA sequence amplification and detection. The system provides real-time analysis of amplified DNA using spectral sensors and features a **Graphical User Interface (GUI)** for easy control and monitoring of PCR protocols.

## Features
- **Multichannel PCR**: Allows simultaneous amplification of multiple DNA samples in real-time.
- **GUI Interface**: Users can define and monitor PCR protocols, track block temperatures, and view real-time amplification results.
- **Thermal Cycler**: Equipped with cartridge heaters and a motorized system to move samples between heating blocks for precise DNA amplification.
- **Fluorescence Detection**: Detects DNA amplification using spectral sensors and displays the results through the GUI.
- **Automatic Control**: Uses PID (Proportional-Integral-Derivative) control for precise temperature regulation across different blocks.
  
## System Components
- **ARM Cortex-A72**: Main processor controlling the system's operations.
- **ATmega-2560**: Microcontroller used for handling temperature and movement control.
- **AS7341 Spectral Sensor**: Used for fluorescence detection in each channel.
- **GUI**: Provides user-friendly control and monitoring of the PCR process.
- **Stepper Motors**: Control the movement of the sample between heating and detection blocks.
- **Cartridge Heater and Thermistor**: Maintain precise temperature control for thermal cycling.
- **LED Source**: Multi-wavelength LED source used for fluorescence detection.

## Setup and Installation

1. **Hardware Setup**: 
   - Ensure all components (thermal blocks, sensors, LEDs, etc.) are securely connected to the system.
   - Power the system using a regulated power supply (12V, 6A or 10A as required).
   
2. **Software Requirements**:
   - The system requires installation of necessary drivers for **Raspberry Pi Compute Module** and **ATmega2560**.
   - Install the GUI software on the control computer.

3. **Running the System**:
   - Power on the system and start the GUI.
   - Define your PCR protocol (number of cycles, temperature set points, duration, etc.) through the GUI.
   - Insert DNA samples into the PCR tubes and place them in the thermal cycler.
   - Start the PCR process and monitor real-time fluorescence through the GUI.

## Usage

1. **Setting up a PCR Protocol**:
   - From the GUI, input the desired temperature and cycle settings.
   - Monitor real-time block temperatures and fluorescence signals.

2. **Fluorescence Detection**:
   - Fluorescence intensity is measured after each cycle. The GUI displays the amplification curve, allowing users to determine DNA amplification in real-time.

## Results

The system provides highly accurate, real-time monitoring of DNA amplification. Fluorescence data from each channel can be saved and used for further analysis.

## Future Improvements

- Expanding the system to support more channels.
- Optimization of fluorescence detection using more advanced sensor technologies.
