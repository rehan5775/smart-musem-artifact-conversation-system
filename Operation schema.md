# Complete Operation Schema

The operation schema follows:

**Pre-condition → Operation → Post-condition**

| ID | Operation | Event / Input | Pre-condition | Post-condition |
|---|---|---|---|---|
| OP01 | Perform Sensor Self-Check | System startup / maintenance request | System is powered on. | Sensor status is verified and faults are identified. |
| OP02 | Check Environmental-Control Devices | System startup / device status request | Control devices are connected. | Availability and status of control devices are known. |
| OP03 | Record Artifact Identification | Artifact ID / identification data | Artifact is registered or presented to the system. | Artifact identification is recorded. |
| OP04 | Load Artifact Environmental Limits | Artifact ID | Artifact identification is available. | Required environmental limits are loaded. |
| OP05 | Monitor Environmental Conditions | Sensor readings | Sensors are operational. | Current environmental conditions are recorded. |
| OP06 | Check Chamber Door Status | Door sensor signal | Chamber is being monitored. | Current door status is known. |
| OP07 | Compare Temperature with Permitted Range | Current temperature + temperature limits | Temperature reading and limits are available. | Temperature condition is determined. |
| OP08 | Correct Abnormal Temperature | Abnormal temperature reading | Temperature is outside the permitted range and controls are available. | Temperature-control action is applied. |
| OP09 | Verify Temperature Recovery | Updated temperature reading | Temperature correction has been applied. | Recovery to the permitted range is confirmed or further action is required. |
| OP10 | Compare Humidity with Permitted Range | Current humidity + humidity limits | Humidity reading and limits are available. | Humidity condition is determined. |
| OP11 | Correct Abnormal Humidity | Abnormal humidity reading | Humidity is outside the permitted range and controls are available. | Humidity-control action is applied. |
| OP12 | Verify Humidity Recovery | Updated humidity reading | Humidity correction has been applied. | Recovery to the permitted range is confirmed or further action is required. |
| OP13 | Detect Significant Vibration | Vibration sensor reading | Vibration sensor is operational. | Harmful vibration is detected or ruled out. |
| OP14 | Suspend Risky Activities | Significant vibration / risk signal | A risky activity is active and a threat is detected. | Risky activity is paused or stopped. |
| OP15 | Verify Vibration Stabilization | Updated vibration reading | Risky activities have been suspended. | Vibration is confirmed safe or additional action is triggered. |
| OP16 | Reduce Light Exposure | High light reading / light threshold | Light sensor and lighting controls are operational. | Light exposure is reduced to a safer level. |
| OP17 | Activate Additional Environmental Controls | Persistent abnormal condition | Normal control action is insufficient. | Additional environmental controls are activated. |
| OP18 | Generate Operator Alert | Critical or abnormal condition | Alert system is available. | Responsible operator receives an alert. |
| OP19 | Switch to Emergency Power | Main power failure | Emergency power source is available. | Chamber systems receive emergency power. |
| OP20 | Record Power-Loss Incident | Power-loss event | Logging system is available. | Power-loss incident is stored with relevant details. |
| OP21 | Verify Chamber Safe Condition | Post-incident sensor/status data | Recovery or incident response is in progress. | Chamber safety status is confirmed. |
| OP22 | Authorize Artifact Removal | Removal request + safety status | Artifact and chamber meet required safety conditions. | Artifact removal is authorized or rejected. |
| OP23 | Record Conservation Activity | Operator action / conservation update | Artifact is registered and the system is operational. | Conservation activity is recorded with time and operator details. |
| OP24 | Check Communication Link | Communication status signal | Monitoring system is powered and communication module is available. | Communication status is confirmed or a communication fault is reported. |
| OP25 | Validate Sensor Reading | New sensor reading | Sensor is active and a reading is available. | Reading is accepted as valid or marked for review. |
