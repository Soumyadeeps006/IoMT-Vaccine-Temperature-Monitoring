# Vaccine Temperature Management using IoMT

## Overview
This project leverages the **Internet of Medical Things (IoMT)** to ensure optimal temperature conditions for vaccine storage and transportation. It integrates IoT-enabled sensors to monitor real-time temperature data and provides automated alerts in case of deviations. A cloud-based system stores and analyzes the data for decision-making and compliance tracking. The solution enhances vaccine efficacy by preventing spoilage due to temperature fluctuations, ensuring transparency and efficiency in vaccine logistics.

## Features
- **Real-time Temperature Monitoring:** IoT-enabled sensors track and report temperature changes.
- **Automated Alerts:** Instant notifications for temperature deviations.
- **Compliance & Reporting:** Ensures adherence to regulatory standards.

## Technology Stack
- **Hardware:** IoT sensors (e.g., DHT22, DS18B20, or industrial-grade temperature sensors)
- **Communication Protocols:** MQTT, HTTP, LoRaWAN
- **Database:** MySQL (connected via JDBC)
- **Backend:** Java (for sensor data handling, connected to MySQL via JDBC)
- **Python (for sensor readings):** Uses `adafruit_dht` library to capture temperature values

## System Architecture
1. **Data Collection:** IoT-enabled sensors continuously monitor temperature using Python (`adafruit_dht` library).
2. **Data Transmission:** Sensor data is processed in Java and stored in MySQL via JDBC.
3. **Cloud Processing:** Data is stored, analyzed, and processed in the cloud.
4. **Dashboard & Alerts:** A web/mobile dashboard visualizes data and triggers alerts.
5. **User Notifications:** SMS, email, or push notifications are sent in case of anomalies.

## Installation & Setup
### Prerequisites
- IoT hardware (temperature sensors)
- Java Development Kit (JDK) installed
- MySQL installed and configured
- Python (with `adafruit_dht` library installed)

### Steps
1. **Clone the Repository**
   ```sh
   git clone https://github.com/Soumyadeeps006/IoMT-Vaccine-Temperature-Monitoring.git
   cd Vaccine-temperature-management-IoMT
   ```
2. **Install Dependencies**
   ```sh
   pip install -r requirements.txt
   ```
3. **Set Up MySQL Database**
   - Create a MySQL database and configure JDBC connection in the Java backend.
4. **Run the Application**
   ```sh
   javac Sensor.java
   java Sensor.java
   python values.py
   ```

## Usage
- **Monitor real-time temperature**
- **Configure alerts and thresholds**
- **Access historical data for analytics**
- **Generate compliance reports**

## Contributing
Contributions are welcome! Follow these steps to contribute:
1. Fork the repository.
2. Create a new branch (`feature-branch`).
3. Commit your changes and push to your fork.
4. Open a pull request for review.

## License
This project is licensed under the GNU General Public License - see the [LICENSE](LICENSE) file for details.

## Contact
For any inquiries or support, reach out to:
- **Email:** soumyadeeps006@gmail.com
- **GitHub Issues:** Open an issue [here](https://github.com/Soumyadeeps006/IoMT-Vaccine-Temperature-Monitoring/issues)
