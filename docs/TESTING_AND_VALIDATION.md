# Testing and Validation

## Evidence standard

This document distinguishes the supplied final-test record from calibrated measurement and formal validation. “Observed” means reported for the documented prototype under the tested conditions. It does not imply certification, statistical reliability, or guaranteed performance in another environment.

The repository contains physical photographs, architecture figures, GPIO evidence, and captured dashboard states. It does not contain raw sensor logs, repeated-trial datasets, oscilloscope traces, certified instruments, or a formal test-laboratory report.

## Documented integrated test session

The integrated prototype completed the documented approximately 30-minute ground test session successfully, with the tested mobility, sensing, dashboard, alarm, display, and communication functions remaining operational under the tested conditions.

No percentage success rate is stated because the evidence does not define a repeated trial count and failure count.

## Observed prototype checks

| Area | Documented observation | Evidence boundary |
|---|---|---|
| Manual mobility | Forward, reverse, left, right, and stop behavior operated in Manual mode | Qualitative integrated test observation |
| Autonomous mobility | Auto mode operated during physical testing | No formal route-completion or avoidance-rate metric |
| Ultrasonic scan | Servo-mounted scan operated | No calibrated angular or distance-accuracy study |
| Focused inspection | LEFT / FRONT / RIGHT inspection operated | Directional function observation |
| Radar | Displayed direction agreed with sensor-head direction | Qualitative agreement, not angular calibration |
| Proximity alarm | Continuous directional proximity warning behavior operated | No formal alarm-latency distribution |
| Environmental telemetry | Temperature, humidity, gas/smoke response, flame, and IR states were presented | Values are not certified metrology data |
| Buzzer | Physical warning output operated | Qualitative output check |
| TFT | Local display operated | Functional observation |
| SoftAP | Direct local dashboard access operated | Prototype wireless observation |
| Home Wi-Fi | Dashboard access through the tested local router environment operated | Environment- and router-dependent |
| Integrated endurance | Robot remained operational for the approximately 30-minute session | One documented session; not a lifetime or reliability test |
| Tested software state | The final competition firmware used for the session was physically tested before this documentation release | Firmware source is not published here |

## Dashboard evidence

![Dashboard overview](../figures/dashboard/dashboard-overview.jpeg)

*Figure 1. Captured Overview state showing live connection, critical hazard indication, Manual mode, stopped/safety-stop state, distance, and front scan direction.*

![Dashboard environment view](../figures/dashboard/dashboard-environment.jpeg)

*Figure 2. Captured Environment state showing temperature, humidity, MQ-2 raw response, and hazard status. Values illustrate a test state and are not calibration references.*

## Network observations

The supplied project record describes:

- direct SoftAP control observed approximately within 15–25 feet; and
- Home Wi-Fi control observed approximately within 50–70 feet or across the tested home environment.

These are approximate observations under the tested conditions. They are not certified communication specifications and should not be generalized to different walls, interference, antennas, routers, clients, or power conditions.

## Measured and displayed values

The dashboard figures visibly include example state values such as 58.3 cm range, 31 °C temperature, and 78% relative humidity. They are preserved as captured interface evidence only. The repository does not claim the values were established with traceable calibrated instruments.

## Claims not established

The available evidence does not establish:

- a statistical success percentage;
- calibrated sensor accuracy;
- motor-speed precision;
- communication performance beyond the observed environment;
- industrial reliability or ingress protection;
- battery endurance beyond the documented session;
- safety certification;
- autonomous navigation coverage; or
- operation of future AI, localization, mapping, camera, ROS 2, or fleet features.

## Recommended future validation

Future work should use defined test protocols with trial counts, pass/fail criteria, timestamped logs, reference instruments, power measurements, controlled obstacle layouts, network signal measurements, and repeatable environmental conditions. Such work would allow quantitative claims without overstating the current evidence.
