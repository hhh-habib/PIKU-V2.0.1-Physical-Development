# Cyber-Physical Systems Research Vision

## What a CPS means here

A cyber-physical system connects:

- a physical robot;
- real-world sensors and actuators;
- embedded computation;
- communication networks;
- software decisions; and
- human supervision.

The cyber and physical parts continuously affect one another. A useful CPS is therefore not only connected; it closes a feedback loop between observations, computation, decisions, and physical change.

## The V2.0.1 feedback loop

PIKU V2.0.1 already demonstrates a compact CPS loop:

1. The environment affects range, temperature, humidity, gas/smoke, flame, and obstacle sensors.
2. The ESP32 acquires and interprets the available signals.
3. State is reported through the TFT, buzzer, alarm logic, radar, and local dashboard.
4. A human operator or autonomous behavior selects an action.
5. Motor and servo outputs change robot position or sensing direction.
6. Sensors observe the resulting environment again.

The direct SoftAP and local-router options add a communication layer without requiring a cloud service. This allows experiments in local supervision, network-dependent control, and distributed monitoring.

## Staged research development

### PIKU V1 — foundational work

- Basic mobile robotics
- Obstacle-avoidance experiments

### PIKU V2 — connected environmental monitoring

- ESP32 connectivity
- Environmental sensing
- Browser-based monitoring direction

### PIKU V2.0.1 — implemented and tested platform

- Expanded safety and environmental sensing
- Improved autonomous behavior
- Servo-mounted ultrasonic radar
- Manual directional inspection
- Direct SoftAP and Home Wi-Fi operation
- Advanced local dashboard
- Modular embedded-system foundation

### PIKU V2.1 — planned research direction

- ESP32-S3 experimentation
- Initial Edge AI studies
- Improved perception
- Additional navigation sensing
- Richer mission intelligence

### PIKU V3 — planned research direction

- Raspberry Pi-class higher-level computing
- ROS 2 integration
- Mapping and localization
- More advanced CPS coordination
- Research-grade modular autonomy

V2.1 and V3 are plans, not implemented V2.0.1 capabilities.

## Longer-term research themes

### Embedded intelligence

Study how local decision-making can become more adaptive while remaining interpretable, resource-aware, and safe.

### Localization and motion

Add calibrated PWM, encoders, heading feedback, odometry, and richer range sensing before making quantitative navigation claims.

### Perception and Edge AI

Evaluate camera or other sensing only after establishing adequate compute, power, data, and validation practices. Edge AI is not present in V2.0.1.

### Mapping and robotics middleware

Explore mapping, localization, ROS 2, and modular mission components on a future higher-level compute layer. Neither SLAM nor ROS 2 is implemented in V2.0.1.

### Distributed sensing and networked CPS

Extend local telemetry toward coordinated environmental monitoring, remote fleet observation, and multi-robot experiments while addressing latency, security, network failure, and human oversight.

## Research discipline

Each stage should preserve the distinction between:

- implemented hardware and software;
- observed prototype behavior;
- calibrated or statistically validated performance; and
- planned research.

This discipline keeps the platform useful for engineering education and credible long-term CPS research.
