# VISTA X


<p align="center">
  <b>Offline Multi-Sensor Safety & Driver Assistance Prototype for Mine Vehicles</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Smart%20India%20Hackathon-2026-1f7a5c?style=for-the-badge">
  <img src="https://img.shields.io/badge/PS-26007-2e5d7b?style=for-the-badge">
  <img src="https://img.shields.io/badge/Platform-Android%20Prototype-3f8f5f?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Prototype-orange?style=for-the-badge">
</p>

> **Smart India Hackathon 2026 · Problem Statement 26007**
>
> **Safe and Efficient Operation of Mine Vehicles in Fog and Low-Visibility Conditions in Open Cast Iron Ore Mines**

VISTA X is a prototype safety-assistance platform for mine vehicles. It combines camera and other sensor inputs, local processing, risk analysis and driver alerts into one modular system.

The larger VISTA concept contains two software layers:

- 🟢 **VISTA X** — driver-side safety assistance
- 🔵 **VISTA A** — centralized monitoring and administration

The system is designed around an **offline-first vehicle-side safety path**, so critical driver-side processing does not have to depend on continuous cloud connectivity.

---

## 📱 Android Prototype

### This is a simple Android prototype

The Android build is intended for **demonstration and early testing**, not as the complete vehicle-side implementation.

### ✅ Available on Android

- 📷 Camera access
- 🎥 Basic camera-based prototype functionality
- 📡 Supported device/sensor communication where implemented
- 🖥️ Prototype UI and system flow
- 🧪 Basic demonstration of the VISTA X concept

### ⚠️ Current Android limitation

**Detailed tracking functionality is not currently supported on Android.**

The Android build should therefore be considered a **simple prototype client**. The fuller tracking/perception workflow is intended for the main supported development environment.

---

# ⬇️ Download VISTA

## Option 1 — Scan the QR code

### 📲 Phone
Open the phone camera or Google Lens and scan the QR code at the top of this README.

It opens:

**GitHub → VISTA → Releases**

From there, download the latest Android APK published by the project.

> The QR code points to the project's **latest GitHub Release page**, so the same QR can remain in posters, presentations and demo booths even when a newer version is published.

---

## Option 2 — Open the GitHub Release page

### 🔗 Latest release

**https://github.com/nitinkharayat/VISTA/releases/latest**

### Installation flow

```text
📱 Scan QR
     ↓
🌐 GitHub Releases
     ↓
📦 Open the latest VISTA release
     ↓
⬇️ Download the Android APK
     ↓
📲 Install
     ↓
🚀 Open VISTA
```

Use the APK published by the official repository.

> **Google Play status:** This prototype is currently distributed through GitHub Releases rather than the Google Play Store.

---

# 🧭 What VISTA Is

VISTA is built as a modular mine-safety concept:

```text
┌────────────────────────────────────────────┐
│              SENSOR / HARDWARE              │
│                                            │
│ 📷 Camera   📡 Sonar   🔦 LiDAR   🌡 Thermal│
│ 🛰 GPS/DGPS   🧭 IMU   📡 Radar            │
│                 │                          │
│          Arduino + ESP8266                │
└─────────────────────┬──────────────────────┘
                      │
                      ▼
┌────────────────────────────────────────────┐
│        LOCAL DATA PROCESSING & FUSION      │
│                                            │
│ 🐍 Python / OpenCV                        │
│ 🔄 Sensor synchronization                  │
│ 🧠 Perception + risk analysis              │
│ 💾 Local storage                           │
└─────────────────────┬──────────────────────┘
                      │
              ┌───────┴────────┐
              ▼                ▼
       🟢 VISTA X          🔵 VISTA A
       Driver View        Admin / Fleet
```

---

# 🟢 VISTA X

## Driver Perspective

VISTA X is the driver-facing safety-assistance layer.

### Core concept

- 📷 Real-time camera perception
- 🔄 Multi-sensor fusion
- 🚧 Object / hazard detection
- ⚠️ Collision-risk alerts
- 🩺 Sensor health awareness
- 🛡️ Degraded-sensor handling
- 📴 Offline vehicle-side processing

The initial prototype follows a **driver-assistance-first** approach.

It is not intended to directly control the mine vehicle.

---

# 🔵 VISTA A

## Centralized Admin / Fleet Monitoring

VISTA A is the central monitoring concept for mine operations.

### Intended functions

- 🚛 Fleet monitoring
- 🚨 Incident records
- 📋 Logs
- 📊 Operational analytics
- 🩺 Sensor/system health
- 🔔 Alerts and reports

### Current demo access

```text
ID       : demo
Password : demo123
```

> These credentials are for the current demo application only. Do not use them for production systems.

---

# 🔧 Hardware & Sensors

The SIH concept is based on a modular sensor architecture.

| Component | Role |
|---|---|
| 📷 Camera | Visual perception |
| 🔦 LiDAR | Distance / spatial information |
| 📡 Sonar | Distance sensing |
| 🌡 Thermal | Heat-based perception |
| 🛰 GPS / DGPS | Position tracking |
| 🧭 IMU | Motion and orientation |
| 📡 Radar | Additional detection |
| 🔌 Arduino | Sensor hub / acquisition |
| 📶 ESP8266 | Communication layer |

The exact hardware configuration can be adapted to the vehicle and deployment environment.

---

# 💻 Technology

| Layer | Technology |
|---|---|
| 🎨 UI | Flutter / Dart |
| 🐍 AI / Backend | Python |
| 👁️ Computer Vision | OpenCV |
| ⚙️ Embedded | C++ |
| 📶 Communication | ESP8266 |
| 🔌 Sensor Hub | Arduino |

---

# 📴 Offline-First Design

A core design principle is to keep the vehicle-side safety path local.

```text
Sensors
   ↓
Local Processing
   ↓
Sensor Fusion
   ↓
Risk Detection
   ↓
Driver Alert
```

This is intended for mine environments where network connectivity can be limited or unavailable.

---

# 🛡️ Sensor-Failure Tolerance

The system concept does not assume that every sensor will always be healthy.

Example:

```text
📷 Camera       ✅
🔦 LiDAR        ✅
🌡 Thermal      ❌
📡 Sonar        ✅

           ↓

   Continue with
 available inputs
```

The system should detect degraded sensor availability and use the remaining valid information where possible.

---

# 🧪 Prototype Status

| Component | Current status |
|---|---|
| 🟢 VISTA X | Public prototype |
| 📱 Android | Simple prototype client |
| 🔵 VISTA A | Demo application |
| 🔧 Hardware | Prototype / development stage |
| 🧠 Full tracking | Main development target |
| 🚛 Production deployment | Future phase |

---

# 🎯 Validation

The project is intended to be validated using measurable KPIs such as:

- 🎯 Detection reliability
- 🚨 False-alert rate
- ⚡ Alert latency
- 🚛 Vehicle cycle time
- ⏱️ Downtime
- 👷 Operator feedback
- 🩺 Sensor health / failure behaviour

The SIH concept defines a **70–80% detection reliability target for controlled pilot conditions**. This is a validation target, not a claim that the field system has already achieved it.

---

# 🗺️ Roadmap

```text
CURRENT
  │
  ├─ 🟢 VISTA X prototype
  ├─ 📱 Android prototype
  ├─ 🔵 VISTA A demo
  └─ 🔧 Sensor-fusion architecture
  │
  ▼
VALIDATION
  │
  ├─ 🧪 Controlled testing
  ├─ 📊 KPI measurement
  ├─ 🩺 Sensor-failure tests
  └─ 👷 Operator feedback
  │
  ▼
PILOT
  │
  ├─ 🚛 Vehicle integration
  ├─ 🌫️ Fog / low-visibility testing
  └─ 🏭 Mine-environment trials
  │
  ▼
DEPLOYMENT
  │
  ├─ 🛡️ Rugged hardware
  ├─ 🚛 Fleet monitoring
  ├─ 📈 Production analytics
  └─ ⚙️ Mine-specific configuration
```

---

# 🔗 Project Links

| Resource | Link |
|---|---|
| 🧑‍💻 Source Repository | https://github.com/nitinkharayat/VISTA |
| 📦 Latest Release | https://github.com/nitinkharayat/VISTA/releases/latest |
| 🐛 Issues | https://github.com/nitinkharayat/VISTA/issues |

---

# 🧑‍💻 For Developers

The project is being developed around a modular separation between:

```text
Flutter / Dart
      │
      ▼
Driver UI
      │
      ▼
Python / OpenCV
      │
      ▼
Perception + Fusion + Risk
      │
      ▼
Embedded / Sensor Layer
      │
      ▼
Arduino + ESP8266 + Sensors
```

The repository is intended to grow with the prototype. Downloadable builds should be distributed through GitHub Releases, while source code and technical documentation remain in the repository.

---

# ⚠️ Prototype Notice

VISTA X is a **hackathon / research prototype**.

It is not a certified safety-critical system and should not be treated as an autonomous vehicle controller.

Real-world deployment would require:

- Controlled testing
- Hardware qualification
- Mine-specific validation
- Safety assessment
- Environmental testing
- Regulatory / operational approval

---

# 👥 Team

**NPSEI_Bug_Busters**

### VISTA X
**Safer Mines · Smarter Operations · Stronger Tomorrow**

---

## ⭐ Support the Project

If you find the project useful:

⭐ Star the repository  
🍴 Fork the project  
🐛 Report issues  
💡 Share improvement ideas

**Repository:**  
https://github.com/nitinkharayat/VISTA
