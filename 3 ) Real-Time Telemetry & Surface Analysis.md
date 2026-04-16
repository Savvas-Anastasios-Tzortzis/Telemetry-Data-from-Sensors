## What is used and why
- Smooth Wood ("The Asphalt"): Provided the most consistent telemetry. The flat, reflective surface allowed for maximum sampling frequency and high precision, representing ideal racing conditions.

- Black Textured Board ("The Kerbs"): Introduced "signal noise" due to physical vibrations and the darker material. This test was crucial for understanding how mechanical instability affects data accuracy.

- Artificial Grass ("The Off-Track"): The most challenging environment. The irregular, porous surface of the grass absorbed part of the ultrasonic waves, leading to "signal absorption" and demonstrating the limits of the sensor in non-ideal conditions.

**Final Verdict**

This project successfully demonstrates how IoT technology can bring Formula 1-style telemetry to micro-scale engineering. By analyzing the data through VS Code, we can differentiate between a clean "racing line" and "track debris" or "off-track" excursions simply by looking at the telemetry spikes.

## Results

**1**. Smooth Wood: The "Optimal Racing Line"

- Result: Extremely stable and consistent telemetry.

- Analysis: On the smooth wooden surface, the ultrasonic waves reflected perfectly back to the sensor. The data stream showed a "clean" signal with zero dropouts, representing the vehicle's behavior on a high-grip, newly paved asphalt track. This was our baseline for maximum precision.

**2**. Black Textured Board: The "Kerb Vibration"

- Result: Increased signal noise and minor data spikes.

- Analysis: Testing on the textured board simulated the car hitting the "kerbs" or "rumble strips." The darker material and the slight surface irregularities caused minor scattering of the sound waves. While the distance was still accurate, the telemetry graph showed "jitter," reflecting the physical vibrations felt by a car when pushing the track limits.

**3**. Artificial Grass: The "Off-Track Excursion"

- Result: High signal absorption and erratic readings.

- Analysis: This was the most challenging test. The artificial grass, being porous and non-uniform, absorbed a significant portion of the ultrasonic pulse rather than reflecting it. The telemetry showed irregular gaps and "ghost" readings, simulating a car losing aerodynamic and sensor efficiency after going off-track into the grass or gravel trap.

**Summary Table**

| Surface Type | F1 Equivalent | Signal Quality | Telemetry Behavior |
|--------------|---------------|----------------|--------------------|
| Smooth Wood | Fresh Asphalt | Excellent | Constant & Linear |
| Textured Board | Track Kerbs | Moderate | Frequent Jitter/Noise |
| Artificial Grass | Grass/Gravel | Low | Erratic/Signal Loss |

**Final Conclusion**

The experiment proved that environmental textures significantly impact IoT sensor reliability. Just like in F1, where engineers adjust for track conditions, our telemetry system requires different filtering levels depending on the "terrain" the RC car is navigating.

