# Smart-Irrigation Controller

Smart-Irrigation Controller is an embedded system designed to optimize irrigation for terraced vineyards, ensuring efficient water distribution and energy use. This project leverages embedded system principles to address real-world agricultural challenges, blending technology with sustainability.

## Project Overview

This system manages the water distribution from a central reservoir to three irrigation zones at different elevations. It involves precise control of water pressure and flow to meet the specific needs of each zone.

### Key Features

- **Central Water Reservoir:** Automatically refills from an underground spring overnight.
- **Pump and Valve System:** Controls water flow to the designated irrigation zones.
- **Water Depth Sensor:** Monitors reservoir levels to prevent overflows and shortages.
- **Servo Mechanism:** Directs water to specific zones, indicated by an RGB LED.
- **PWM Signal:** Adjusts pump motor speed for optimal water pressure.
- **Ultrasonic Sensor:** Measures water depth accurately.
- **Seven-Segment Display:** Shows real-time water level percentages.
- **Potentiometer:** Allows manual adjustment of pump RPM.
- **MCU Timer:** Simulates real-time operation on a scaled timeline.

### MCU Timer Board
<img width="810" alt="MCU Timer Board" src="https://github.com/Karnan123/Smart-Irrigation-Controller/blob/main/Timer_Board_Picture.jpg?raw=true">

## System Operation

1. **Filling the Reservoir:**
   - The reservoir is replenished overnight via an inlet pipe controlled by a servo, indicated by a purple RGB LED.

2. **Irrigation Process:**
   - The system directs water to one of three zones based on a schedule.
   - Pump speed is adjusted using PWM signals to meet the required water pressure for each zone.

3. **Zone Specifications:**
   - **Zone 1:** 50,000 gallons/day; HEAD: 25 feet.
   - **Zone 2:** 30,000 gallons/day; HEAD: 50 feet.
   - **Zone 3:** 14,000 gallons/day; HEAD: 60 feet.
   - **Inlet:** HEAD: 40 feet from the spring.

### Setup and Run Modes

- **Setup Mode:**
  - Configure wall clock times for inlet and zones (0-23 hours).
  - Transition to run mode by pressing the blue B1 button.

- **Run Mode:**
  - Operates according to the configured schedule.
  - Adjusts pump speed and monitors reservoir levels to maintain efficient operation.
  - Halts system operation and indicates status via LEDs in special events.

## Energy Efficiency

- The pump’s power consumption is managed to ensure energy-efficient operation, with calculations based on RPM and runtime.

## High-Level Design

This project highlights the potential of embedded systems in resource conservation. By integrating sensors, actuators, and intelligent control, Smart-Irrigation Controller ensures sustainable water management in agriculture.
