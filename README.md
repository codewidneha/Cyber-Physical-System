
# Cyber-Physical System Monitoring

## Overview

This project simulates a Cyber-Physical System (CPS) designed to monitor sensor data for potential anomalies (such as cyber theft or system malfunctions). It incorporates encryption for data security, anomaly detection, control actions based on detected anomalies, and real-time data visualization. 

The system fetches sensor data, analyzes it, and displays alerts or control actions based on predefined thresholds. It also uses encryption (via `cryptography` library) to secure sensor data.

---

## Features

- **Sensor Simulation**: Simulates sensor data with both normal and abnormal values.
- **Anomaly Detection**: Detects anomalies if sensor data exceeds a set threshold.
- **Data Encryption**: Uses the `cryptography` library for secure data encryption and decryption.
- **Control Actions**: Takes control actions (e.g., lockdown) when anomalies are detected.
- **Real-Time Visualization**: Visualizes sensor data and thresholds with live updating plots.
- **Console-Based UI**: Displays the sensor data, analysis, control actions, and encrypted data in the console.

---

## Installation

1. Install the necessary Python libraries:

```bash
pip install cryptography matplotlib
```

---

## Usage

### Running the System

To run the system, simply execute the script. It will simulate data fetching, detect anomalies, encrypt/decrypt data, and display control actions:

```bash
python main.py
```

### Real-Time Visualization

The system also includes live data visualization. The plot updates in real-time as the sensor data is generated and processed.

---

## Example Output

```plaintext
Cyber-Physical System - Security Monitor

Fetching sensor data...
Sensor Data: 109
Encrypted Data: gAAAAABnTsd5WwCBkIdJoRaUjrV22xI4Kd0Kab7ErcZ842AOZ07nQZScHcy8TEvyWNy9-itCke81YOd9Lb7qYGevXwnqxbDHdw==
Analysis: System Normal
Decrypted Data: 109
Control Action: System running smoothly.

...

Monitoring session completed.
```

---

## How It Works

1. **Sensor Data Generation**: Random values between 100 and 200 are generated. Values above 150 are considered abnormal (simulating potential cyber theft).
2. **Data Encryption/Decryption**: The sensor data is encrypted using the `cryptography` library. It is decrypted for display purposes after being processed.
3. **Anomaly Detection**: If the sensor data exceeds a threshold of 150, an alert is triggered.
4. **Control Actions**: If an anomaly is detected, control actions such as "Lockdown system" are initiated. Otherwise, the system runs smoothly.
5. **Real-Time Plotting**: A live plot visualizes sensor data, the threshold, and system status.

---

## Files

- `main.py`: Main script containing the implementation of sensor data simulation, encryption, anomaly detection, control actions, and visualization.

---

## Dependencies

- Python 3.x
- `cryptography`
- `matplotlib`
- `random`
- `time`

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
