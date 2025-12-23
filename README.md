# 🤖 Hello Reachy Mini

**Exploring Reachy Mini from an Engineering Perspective**

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

</div>

---

## 📋 Table of Contents

- [Platform Overview](#-platform-overview)
- [Quick Start](#-quick-start)
- [System Specifications](#-system-specifications)
- [Resources](#-resources)

---

## 🎯 Platform Overview
| **🤖 Reachy Mini (Wireless)** | **🔌 Reachy Mini Lite** | **💻 Simulation** |
| :---: | :---: | :---: |
| The full autonomous experience.<br>Raspberry Pi 4 + Battery + WiFi. | The developer version.<br>USB connection to your computer. | No hardware required.<br>Prototype in MuJoCo. |
| 👉 [**Go to Wireless Guide**](docs/platforms/reachy_mini/get_started.md) | 👉 [**Go to Lite Guide**](docs/platforms/reachy_mini_lite/get_started.md) | 👉 [**Go to Simulation**](docs/platforms/simulation/get_started.md) |

---

## 🚀 Quick Start

### Remote Access (SSH)
```bash
ssh pollen@reachy-mini.local
# Default password: root
```

### Control Interface
Access the robot control landing page:
```
http://reachy-mini.local:8000/
```

### SDK Repository
Official Reachy Mini SDK: [pollen-robotics/reachy_mini](https://github.com/pollen-robotics/reachy_mini)

---

## 📊 System Specifications

> **System Audit Date:** December 24, 2025  
> **Hostname:** `reachy-mini`
### 🐧 Operating System & Kernel
| Parameter | Value / Result | Notes |
| :--- | :--- | :--- |
| **OS Name** | Debian GNU/Linux 13 (trixie) | *Newer "Testing" branch of Debian* |
| **Kernel Version** | `6.12.47+rpt-rpi-v8` | *Raspberry Pi optimized kernel (64-bit)* |
| **Architecture** | arm64 (aarch64) | |

## 2. Hardware Specification
| Parameter | Value / Result | Details |
| :--- | :--- | :--- |
| **⚙️ CPU Model** | Cortex-A72 (4 Cores) | *Raspberry Pi 4 Model B* |
| **CPU Speed** | 600 MHz (Min) - 1.5 GHz (Max) | |
| **RAM (Total/Used)** | Total: 3.7Gi (~4GB) / Used: 762Mi | *Healthy memory usage (approx 20%)* |
| **USB Devices** | - Pollen Robotics Reachy Mini Audio<br>- Terminus Technology Inc. Hub<br>- Linux Foundation 2.0 root hub | *Microphones/Speakers detected as "Reachy Mini Audio"* |
| **Audio Input** | Card 0: Reachy Mini Audio | *Subdevice #0 active* |
| **Audio Output** | Card 0: Reachy Mini Audio | *Also available: vc4-hdmi-0 / vc4-hdmi-1* |

### 💾 Storage
| Parameter | Value / Result |
| :--- | :--- |
| **Filesystem Size** | 14G (Total Partition Size) |
| **Used Space** | 9.7G (74% Used) |
| **Available Space** | 3.5G |
| **Device Type** | SD Card (`mmcblk0`) |

### 🌐 Network Configuration
| Parameter | Value / Result |
| :--- | :--- |
| **Hostname** | `reachy-mini` |
| **Status** | Network Active (SSH Connected) |

### 🐍 Reachy Software Environment
| Parameter | Value / Result | Notes |
| :--- | :--- | :--- |
| **Python Version** | Python 3.13.5 | |
| **Reachy App Status** | **Active (Running)** | *Service: reachy-mini-daemon* |
| **Execution Path** | `/venvs/src/reachy_mini/` | *Software runs inside virtual environment.* |
| **Running Tasks** | - `launcher.sh`<br>- `reachy_mini_conversation_app` | *Conversation AI is currently active.* |

### 🔌 Active Network Services (Open Ports)
| Port | Protocol | Service / Process | Description |
| :--- | :--- | :--- | :--- |
| **8000** | TCP | `python` (PID 930) | **Reachy Mini Daemon API**<br>Core control interface for the robot. |
| **7860** | TCP | `python` (PID 1491) | **Conversation App UI**<br>Standard port for Gradio web interfaces (AI Chat). |
| **22** | TCP | `sshd` (PID 929) | **SSH Server**<br>Remote command line access. |

### Network Endpoints
| Endpoint | Purpose |
|----------|---------|
| `http://reachy-mini.local:8000/` | Robot Control API |
| `http://reachy-mini.local:7860/` | Conversation App UI (Gradio) |
| `ssh pollen@reachy-mini.local` | SSH Access |

<img width="1251" height="1321" alt="image" src="https://github.com/user-attachments/assets/64d1f17f-5dd0-4e1c-b361-46e0673bce39" />

---
## Reachy Mini Conversation App
- Conversation app uses OpenAI API Key.
- [Github](https://github.com/pollen-robotics/reachy_mini_conversation_app)

---
## 📚 Resources

### Official Documentation
- [Reachy Mini SDK Repository](https://github.com/pollen-robotics/reachy_mini)
- [Wireless Setup Guide](docs/platforms/reachy_mini/get_started.md)
- [Lite Version Guide](docs/platforms/reachy_mini_lite/get_started.md)
- [Simulation Guide](docs/platforms/simulation/get_started.md)

<div align="center">

**Made with ❤️ for Reachy Mini Development**

*System audit data generated: December 24, 2025*

</div>


