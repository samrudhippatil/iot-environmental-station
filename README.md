# IoT Environmental Station - CIS600 Assignment 3

This project demonstrates a simulated IoT-based environmental monitoring system using MQTT and ThingSpeak. The system simulates sensor data (temperature, humidity, CO₂) and transmits it to a cloud-based platform for storage and visualization.

## 📌 Project Components

- `virtual_station.py`: Simulates sensor readings and publishes them to a public MQTT broker (HiveMQ) and ThingSpeak.
- `thingspeak_plot.ipynb`: Retrieves and visualizes the last 5 hours of data from ThingSpeak using their REST API.
- `screenshots/`: Contains output screenshots for documentation and verification purposes.

## 🔧 Requirements

Install the following Python packages:

`pip install paho-mqtt requests pandas matplotlib`

🚀 How to Use
Run the Virtual Station
- run all cells of Virtual Station.ipynb
This script sends random sensor data every few seconds to the MQTT broker and also posts it to your ThingSpeak channel.

View Live Graphs
- Log in to your ThingSpeak channel.
- Observe temperature, humidity, and CO₂ plots in real time.

Visualize Historical Data
- Open thingspeak_plot.ipynb in Jupyter Notebook.
- Run all cells to retrieve and display the last 5 hours of sensor data as a combined dashboard figure.

🧩 Configuration
Update the following before running:

In virtual_station.py, set your THINGSPEAK_API_KEY.

In thingspeak_plot.ipynb, set your CHANNEL_ID and READ_API_KEY.

🌐 Cloud Services Used
HiveMQ Public MQTT Broker: For lightweight message transmission.

ThingSpeak: For cloud data storage, visualization, and API access.

👤 Author
Samrudhi Patil
