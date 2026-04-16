## Key Connections & Signal Integrity

Instead of a simple "plug-and-play" setup, the wiring includes critical features to ensure long-term stability:

- Logic Level Protection: Since the HC-SR04 sensor outputs a 5V signal and the Wemos D1 Mini operates at 3.3V, I implemented a Voltage Divider. Using a specific resistor network (1kΩ and 2kΩ), the voltage is stepped down to safe levels, protecting the ESP8266 from electrical stress.

- Dual-Channel Data Path: The system utilizes dedicated Trigger and Echo pins. The Trigger initiates the ultrasonic pulse, while the Echo pin captures the returning signal, allowing for microsecond-precision timing.

- Common Ground Architecture: All components share a common ground (GND) to eliminate electrical noise and ensure that the telemetry data remains consistent during high-speed sampling.

**Optimized for Mobility**

The entire circuit is designed to be vibration-resistant for RC car mounting. By keeping the wiring compact and utilizing a centralized power rail, the system maintains a steady Wi-Fi connection and accurate distance readings while the vehicle navigates different surfaces.
