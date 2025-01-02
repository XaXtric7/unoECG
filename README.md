# Arduino ECG Monitoring System 💓

This project demonstrates a simple ECG (Electrocardiogram) monitoring system using Arduino. The system reads analog signals from a connected ECG sensor and outputs the data over serial communication. It also includes lead detection functionality to ensure proper sensor contact.

## 📌 Features

- **Analog Signal Reading:** Captures ECG data through the analog input pin (A0).
- **Leads-Off Detection:** Monitors the status of the ECG leads and alerts if they are disconnected.
- **Serial Communication:** Sends ECG data or alerts to a connected device (e.g., a computer) for monitoring and graphing.

## 🛠️ Hardware Components

- Arduino Uno
- ECG Sensor Module (e.g., AD8232)
- Electrodes for ECG signal capture
- Jumper Wires and Breadboard

## 📂 How It Works

1. **Initialization:** Serial communication is initialized at 9600 baud. The system also sets up pins 10 and 11 for lead detection.
2. **Lead Detection:** If either lead is disconnected, the system outputs `!` to the serial monitor.
3. **Data Reading:** When leads are connected, the system reads analog data from pin A0 and outputs the values to the serial monitor.
4. **Delay:** A short delay (10ms) is introduced to avoid saturating the serial communication channel.

## 📋 Code Explanation

- **Setup:** Initializes the serial communication and configures lead detection pins as inputs.
- **Loop:** Continuously checks for lead connection status and reads the ECG signal from the analog pin. Outputs either the ECG data or a warning (`!`) for disconnected leads.

## 🎯 Applications

- Basic ECG signal monitoring for educational purposes.
- Demonstration of analog signal processing and serial communication with Arduino.
- Building blocks for more advanced bio-medical projects.

## 🚀 Future Enhancements

- Visualize ECG data using Python or MATLAB for real-time graphing.
- Add filtering for noise reduction in the ECG signal.
- Implement data logging for detailed analysis.
- Introduce wireless communication for remote monitoring.

---

This project is an excellent starting point for understanding ECG signal processing and exploring bio-medical applications with Arduino.
