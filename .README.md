# Telemetry-Data-from-Sensors
With the evolution of software, all motorsport categories have changed a lot. In modern Formula 1, cars utilize over 300 sensors to stream live performance data to the pit wall. This project translates that professional telemetry philosophy into a micro-scale IoT application by mounting a sensor suite on an RC vehicle, simulating a mobile "test bench" for real-time data acquisition. 

## Hardware Stack
| Name | Description |
|------|-------------|
| Wemos D1 Mini (ESP8266) | The core processor with integrated Wi-Fi, mounted on the RC chassis for wireless data streaming. |
| HC-SR04 Ultrasonic Sensor | Positioned at the front of the vehicle to act as "eyes," measuring proximity and obstacle distance. |
| Signal Protection | A custom Logic Level Voltage Divider (1kΩ & 2kΩ resistors) to safely bridge the sensor’s 5V output with the microcontroller’s 3.3V input. |
| Power | Independent battery pack to ensure the telemetry system operates without draining the RC car's main motor. |

## How it works
As the RC car moves, the system captures distance measurements at high frequencies (up to 100Hz) and broadcasts them instantly over Wi-Fi. This creates a live, wireless telemetry feed, allowing a "race engineer" to monitor the vehicle's surroundings from any laptop or smartphone in real-time.

## System Architecture & Hardware Integration
In motorsport, reliability is everything. For this project, the hardware was integrated using a "Modular Design" approach on a breadboard, ensuring that the sensor data remains stable even when the RC car is in motion. The focus was on creating a clean signal path between the ultrasonic sensor and the microcontroller.

## Development Environment & Data Link
To manage the complexity of real-time telemetry, I transitioned from the standard Arduino IDE to a professional development stack: VS Code integrated with PlatformIO. This environment serves as the "Digital Pit Wall," allowing for advanced code management and high-speed communication.

## Real-Time Telemetry & Surface Analysis
The final stage of the project involved mounting the system on an RC vehicle to test sensor performance across three distinct simulated racing environments. The goal was to analyze how different textures affect the "Echo" signal return.
