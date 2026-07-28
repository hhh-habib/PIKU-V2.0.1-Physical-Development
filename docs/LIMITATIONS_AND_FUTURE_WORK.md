# Limitations and Future Work

## Present limitations of PIKU V2.0.1

### Motion and navigation

- No closed-loop motor-speed control
- No PWM speed regulation in the current version
- Directional motor commands and timed/open-loop turning
- No wheel encoders
- No compass or heading feedback
- No odometry
- No SLAM or map generation
- No quantified motion accuracy

### Perception and obstacle coverage

- One servo-mounted ultrasonic ranging sensor
- No rear obstacle sensor
- No camera-based perception
- No onboard Edge AI in V2.0.1
- Directional sensing depends on servo position and the field of view of the installed sensors

### Environmental sensing

- MQ-2 behavior requires warm-up and environment-specific calibration
- Available readings are not certified metrology data
- Gas, smoke, flame, and obstacle indications are prototype warning functions only

### Mechanical, electrical, and operational limits

- Prototype wiring and mechanical structure are not industrialized
- No documented environmental sealing or ingress rating
- Wi-Fi range depends on layout, interference, client, and router
- Battery runtime depends on battery condition, load, regulator efficiency, motion, and radio use
- The documented endurance result is one approximately 30-minute integrated session, not a reliability specification

## PWM limitation and design priority

PIKU V2.0.1 prioritizes reliable system integration, sensing, communication, safety behavior, and autonomous/manual control validation. Variable motor-speed control through PWM was intentionally deferred because this version serves as a developing prototype within a broader CPS research roadmap.

The L298N enable jumpers remain installed in the present configuration. GPIO 25 and GPIO 14 are reserved for possible future right/left enable control; they do not provide active speed regulation in V2.0.1. The current platform therefore does not claim precise speed control.

Future revisions may introduce calibrated PWM control, encoder-based odometry, heading feedback, and closed-loop motion control.

## Planned future work

- PWM and closed-loop motion control
- Rear obstacle sensing
- Compass and encoder feedback
- Improved power management and runtime characterization
- Edge AI experiments
- Camera-based perception
- Mission logging and repeatable test datasets
- Mapping and localization
- ROS 2 integration
- Raspberry Pi-class computing
- Remote fleet monitoring and networked CPS experiments
- Stronger mechanical enclosure and wiring harnesses
- Defined safety states for network or sensor failure

## Validation priorities

Future development should pair each feature with test criteria. Examples include repeatable course layouts for navigation, reference instruments for environmental sensing, timestamped network and alarm logs, controlled battery discharge tests, and defined failure/recovery scenarios.

Planned features should be moved into the implemented list only after physical integration and documented testing.
