# Engineering Contribution

## Contribution statement

PIKU V2.0.1 contributes a physically realized, integrated embedded-robotics platform rather than a new commercial sensor module. Its engineering value lies in how mobility, sensing, communication, monitoring, visualization, safety behavior, and operator interaction are coordinated within one developing research system.

## System integration

The platform brings together:

- a rechargeable mobile power architecture;
- a four-motor drive system;
- environmental and hazard sensing;
- servo-directed ultrasonic inspection;
- manual and autonomous operating modes;
- on-robot TFT and buzzer feedback;
- real-time local telemetry;
- a mobile-friendly browser dashboard; and
- both direct robot Wi-Fi and configured local-router operation.

This integration creates a coherent sensing–decision–action loop. Physical state is measured, interpreted by embedded control, reported to the operator, and used to influence motor, servo, display, and alarm behavior.

## Transition toward a research platform

The design advances the PIKU line beyond a basic mobile obstacle-avoidance robot. V2.0.1 is structured as an experimental base on which navigation, perception, communication, and CPS ideas can be tested incrementally.

Important platform-level developments include:

- directional ultrasonic inspection without rotating the entire chassis;
- explicit LEFT / FRONT / RIGHT focused inspection;
- radar visualization aligned with sensor-head direction;
- multi-sensor hazard awareness;
- physical and browser-based feedback;
- manual override and autonomous operation in the same prototype;
- locally served telemetry without a mandatory cloud service; and
- documented boundaries between present functions and planned research.

## Human-machine interface

The dashboard translates embedded state into a compact mobile interface. It presents movement controls, operating state, range direction, environmental readings, alarms, and connectivity information. The TFT and buzzer maintain local feedback when a browser is not being observed.

## Physical realization and testing

The contribution includes component selection, mechanical placement, power distribution, wiring integration, signal assignment, physical assembly, and integrated ground testing. The documented test record exercises the robot as a connected whole rather than as isolated modules.

## Research value

PIKU V2.0.1 establishes a modular development path toward:

- calibrated motor control and feedback;
- localization and mapping;
- richer perception and Edge AI;
- higher-level mission logic;
- ROS 2 and Raspberry Pi-class computing; and
- distributed or multi-robot cyber-physical systems.

Those items remain planned. The current contribution is the working physical/cyber foundation needed to investigate them responsibly.

## Attribution boundary

The researcher does not claim invention of the ESP32, L298N, HC-SR04, DHT22, MQ-2, ST7789, SG90, or other commercial modules. The original contribution is primarily:

- system integration;
- embedded architecture;
- physical realization;
- iterative testing;
- human-machine interface development; and
- creation of an extensible robotics/CPS research platform.

## Researcher

**Md Habibur Rahman Habib**  
Research Assistant  
First Author and Chief Robotics Engineer
