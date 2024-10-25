# OpenGardener 🌱

An open-source smart greenhouse platform that democratizes sustainable agriculture through accessible technology. OpenGardener combines modular hardware designs, intelligent monitoring systems, and community-driven knowledge sharing to make precision agriculture available to everyone.

![License](https://img.shields.io/badge/license-Apache%202.0-green)
![Status](https://img.shields.io/badge/status-prototype-orange)

## 🎯 Vision

OpenGardener aims to make sustainable agriculture accessible to everyone - from hobby gardeners to small-scale farmers - through open-source smart greenhouse technology. Our platform combines hardware designs, sensor systems, and cloud connectivity to create an intelligent growing environment that's both affordable and scalable.

## 🚀 Current Features (Prototype)

- Modular greenhouse design with 3D-printable components
- Basic environmental monitoring system
  - Temperature & humidity sensing
  - Soil moisture monitoring
  - Light level detection
- Single Raspberry Pi-based control system
- Python-based web dashboard and API
- Local k3s deployment for future scalability

## 🛠️ Technology Stack

### Software
- **Backend & Frontend**: Python 3.11+
  - FastAPI for REST API
  - FastHTML for server-side rendered UI
  - Pydantic for data validation
  - SQLModel for database management
- **Database**: SQLite (local)
- **IoT Communication**: MQTT
- **Infrastructure**: k3s (single-node)

### Hardware (Minimal Setup)
- 1x Raspberry Pi 4 (4GB+ RAM recommended)
- Basic Sensor Kit:
  - DHT22 (Temperature/Humidity)
  - Capacitive Soil Moisture
  - TSL2591 (Light)
  - Optional: CO2, pH sensors
- MicroSD card (32GB+ recommended)
- 5V/3A Power Supply

## 🌱 Getting Started

### Hardware Setup
1. Flash Raspberry Pi OS Lite (64-bit) to SD card
2. Connect sensors to GPIO pins:
   - DHT22 → GPIO4
   - Soil Moisture → GPIO17
   - Light Sensor → I2C (GPIO2/GPIO3)
3. Power up the Raspberry Pi

### Software Prerequisites
- Raspberry Pi OS Lite (64-bit)
- Python 3.11+
- k3s (optional for container management)
- Git

## 📜 License

This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details.
