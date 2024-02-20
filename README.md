# Ultrasonic-Tank-Level-Monitor
**README.md**

### Ultrasonic Tank Level Monitor

This project implements an ultrasonic tank level monitoring system using an Arduino UNO R3 and an ultrasonic distance sensor. It provides real-time monitoring of the fluid level in a tank and alerts the user when the tank is full or empty using LEDs.

#### Materials Required:
- Arduino UNO R3
- Ultrasonic Distance Sensor (e.g., HC-SR04)
- LEDs
- Resistor (appropriate for the LEDs)
- Jumper Wires

#### Software Required:
- Arduino IDE (for local development)
- TinkerCad (for simulation and testing)
- Python (for data analysis, optional)
- Google Colab (for collaborative data analysis, optional)

#### Installation and Setup:
1. **Hardware Setup**:
   - Connect the ultrasonic sensor to the Arduino board as follows:
     - VCC pin to 5V
     - GND pin to GND
     - Trigger pin to digital pin 2
     - Echo pin to digital pin 3
   - Connect LEDs to the appropriate output pins of the Arduino board. Use a resistor in series with each LED to limit the current.

2. **Software Setup**:
   - Install the Arduino IDE from [here](https://www.arduino.cc/en/software).
   - Set up TinkerCad account and access the TinkerCad Circuits platform for simulation.
   - Optionally, install Python on your local machine for data analysis.
   - Optionally, set up a Google Colab account for collaborative data analysis.

3. **Programming**:
   - Copy and paste the provided Arduino sketch into the Arduino IDE.
   - Verify and upload the sketch to your Arduino board.

4. **Testing and Simulation**:
   - Use TinkerCad Circuits to simulate the behavior of the system.
   - Adjust parameters and test different scenarios to validate the system's performance.

5. **Data Analysis (Optional)**:
   - Use Python and libraries like NumPy, Matplotlib, or Pandas for data analysis if required.
   - Collaborate on data analysis tasks using Google Colab for sharing and collaborative editing.

### Screenshots:

<img width="950" alt="1" src="https://github.com/aditiravindranayak/Ultrasonic-Tank-Level-Monitor/assets/109815646/b57d1438-4981-4c3c-a23b-6d92e6f016fd">


<img width="950" alt="2" src="https://github.com/aditiravindranayak/Ultrasonic-Tank-Level-Monitor/assets/109815646/43cd84e7-a3fb-4a76-bb35-069bf70ba28d">

How It Works:

The sketch reads the distance measured by the ultrasonic sensor.
- Based on the distance, it determines whether the tank is full or empty.
- If the tank is full (distance <= 40), it activates two output pins (8 and 9) and plays a tone.
- If the tank is empty (distance >= 300), it deactivates one of the output pins (8).

#### Usage:
- Power on the Arduino board and observe the behavior of the LEDs indicating the tank level.
- Monitor the serial output for real-time feedback on the tank level.

#### Note:
- Ensure proper wiring and component compatibility before uploading the sketch to your Arduino board.
- Customize the Arduino sketch as needed to adapt it to specific tank dimensions or requirements.
- Experiment with different visualization and analysis techniques using Python and Google Colab to gain insights from the collected data.

Feel free to modify the project according to your requirements and expand upon it as needed. Happy tinkering!
