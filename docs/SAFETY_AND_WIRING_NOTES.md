# Safety and Wiring Notes

## Scope

PIKU V2.0.1 is a supervised research prototype. This document highlights important risks but is not a substitute for component datasheets, qualified electrical review, battery-manufacturer guidance, or applicable laboratory rules.

## Before connection

- Verify every supply voltage and signal level before connection.
- Confirm battery polarity, regulator polarity, and connector orientation.
- Adjust and measure the LM2596 output before connecting the ESP32 or peripherals.
- Confirm the actual requirements of each installed module; similar-looking boards may differ.
- Use a common ground between the controller, driver, sensors, display, servo, buzzer, and power system.
- Inspect wiring for loose strands, abrasion, overheated connectors, and accidental shorts.

## ESP32 signal protection

- ESP32 GPIO is not 5 V tolerant.
- Use correct HC-SR04 ECHO level protection; the divider belongs on ECHO, not TRIG.
- Confirm that MQ-2 **AO** is connected to the intended ADC path; do not confuse AO with **DO**.
- Ensure MQ-2 AO remains within the ESP32 ADC input range.
- Verify flame and IR module output voltages before connecting them to GPIO.
- Remember that GPIO 34, 35, 36, and 39 are input-only on the documented ESP32 arrangement.

## Battery and power safety

- Use charging equipment appropriate to the exact 3S lithium-ion battery configuration and protection arrangement.
- Do not infer charger compatibility from connector shape alone.
- Do not charge damaged, swollen, hot, leaking, mismatched, or otherwise questionable cells.
- Do not bypass required battery protection.
- Prevent short circuits and exposed conductive contact.
- Supervise charging and follow the cell, charger, and protection-board manufacturers' instructions.
- Stop operation if wiring, cells, regulators, or the motor driver become abnormally hot.

This repository does not claim that any particular charging method is universally safe.

## Motor and mechanical safety

- Lift the drive wheels clear of the surface during initial motor-direction or software testing.
- Stabilize the chassis before energizing lifted wheels.
- Keep hands, hair, clothing, and tools clear of wheels, shafts, and gears.
- Provide a readily accessible means to remove power.
- Operate in an open supervised area away from stairs, traffic, water, flame, and fragile objects.
- Stop the platform if control or network behavior becomes uncertain.

## Sensor and alarm limitations

- Gas and flame sensing are prototype warning functions, not certified life-safety systems.
- Do not use PIKU as a replacement for certified fire, smoke, carbon-monoxide, or gas detectors.
- Do not intentionally expose the prototype to dangerous gas, smoke, or open flame without an approved controlled laboratory procedure.
- MQ-2 response depends on warm-up, calibration, cross-sensitivity, placement, airflow, temperature, and humidity.
- Ultrasonic and IR sensing can be affected by object angle, surface, geometry, ambient conditions, and blind zones.

## Operating responsibility

Operate the robot under supervision. The operator is responsible for verifying the physical build, safe test environment, battery condition, wiring, and emergency stop/removal of power before each session.
