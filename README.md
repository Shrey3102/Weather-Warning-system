# Weather Monitoring System using IFTTT, IoT, ESP32, and OpenWeatherMap

![Weather Monitoring System](weather_monitoring_system.jpg)

The Weather Monitoring System is a project that utilizes the power of Internet of Things (IoT) and IFTTT (If This Then That) platform to gather weather data using the ESP32 microcontroller and display it through the OpenWeatherMap API. This system provides real-time weather information for a specific location and enables users to take actions based on weather conditions.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Weather Monitoring System is designed to fetch weather data using the ESP32 development board and connect to the OpenWeatherMap API to provide accurate weather information. By utilizing IFTTT, users can automate actions like sending notifications, adjusting connected devices, or triggering events based on specific weather conditions.

## Features

- Real-time weather monitoring
- Integration with OpenWeatherMap API
- Automated actions using IFTTT applets
- Customizable location tracking
- Support for various weather parameters

## Requirements

- ESP32 development board
- Arduino IDE
- Wi-Fi connection
- OpenWeatherMap API key
- IFTTT account
- Basic knowledge of programming and electronics

## Setup Instructions

1. **Clone the Repository**: Clone this repository to your local machine using the following command:
    ```
    git clone https://github.com/Shrey3102/weather-monitoring-system.git
    ```

2. **Open Arduino IDE**: Make sure you have the Arduino IDE installed and open the cloned project folder.

3. **Install Libraries**: Install the necessary libraries using the Arduino Library Manager:
    - ESP32 board library
    - Adafruit Unified Sensor library
    - DHT sensor library (if using DHT sensors)
    - IFTTTWebhook library

4. **Update Configuration**: Open the `config.h` file and update the following variables:
    - `WIFI_SSID` and `WIFI_PASSWORD`: Your Wi-Fi credentials.
    - `OPENWEATHERMAP_API_KEY`: Your OpenWeatherMap API key.
    - `IFTTT_EVENT_NAME`: The name of the event to trigger on IFTTT.
    - `LOCATION_LATITUDE` and `LOCATION_LONGITUDE`: Latitude and longitude of your desired location.

5. **Upload Code**: Select the appropriate ESP32 board from the Arduino IDE's board menu. Compile and upload the code to your ESP32.

6. **IFTTT Setup**:
    - Create an account on [IFTTT](https://ifttt.com/) if you don't have one.
    - Create a new applet:
        - **If This**: Choose a trigger service, e.g., Weather Underground.
        - **Then That**: Choose an action service, e.g., Notifications.
        - Configure the action based on your needs and the trigger data.

7. **Monitor Weather**: Once the code is uploaded and the system is running, you will start receiving weather data through the OpenWeatherMap API and triggering IFTTT applets based on the specified conditions.

## Usage

- The ESP32 will periodically fetch weather data and display it on the connected display or send it to a cloud service.
- IFTTT applets can be used to automate actions like sending notifications to your phone, adjusting smart thermostats, or any other IoT-related tasks.

## Contributing

Contributions to the Weather Monitoring System project are welcome! Feel free to submit pull requests for bug fixes, new features, or improvements. Please follow the project's coding standards and guidelines.

## License

This project is licensed under the [MIT License](LICENSE).
