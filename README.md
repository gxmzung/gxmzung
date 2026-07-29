<div align="center">

# Lee Youngjun / 이영준

### Computer Engineering · Autonomous UAV Systems · Embedded & Mission Software

**UAV / VTOL · ROS2 / PX4 · Embedded Linux · Telemetry · Mission Autonomy · System Integration**

</div>

---

## About Me

I am a Computer Engineering student interested in **real-world autonomous aerospace and unmanned systems**.

My background began around electronics and embedded systems, including circuit/PCB production workflows, Linux-based equipment, firmware testing, and hardware-software integration.  
After entering university, I have been expanding that experience toward **UAV mission systems, ROS2/PX4, telemetry, disaster-response platforms, and autonomous-system software**.

I am especially interested in problems where software must work together with **flight controllers, onboard computers, sensors, communications, and operators in real environments**.

Rather than focusing only on a single software layer, I want to understand and build the full flow:

```text
Sensors / Hardware
        ↓
Embedded Linux / Interfaces
        ↓
ROS2 / PX4 / MAVLink
        ↓
Telemetry / State Management
        ↓
Perception / Mission Logic
        ↓
GCS / Operator Interface
        ↓
Autonomous Mission System
```

---

## Current Focus

### 🛩️ Korea Robot Aircraft Competition — SkyEdge
**Software · System Integration · PM | 2026 - Present**

Currently participating in the 24th Korea Robot Aircraft Competition.

System components include:

- Pixhawk 6X flight controller
- Jetson Orin Nano onboard computing
- Intel RealSense D435i
- RTK-GNSS / IMU / telemetry
- GCS and mission-control software
- Vision and autonomous mission functions

My main interest is connecting these components into a **reliable UAV mission system**, rather than treating flight control, vision, communications, and software as isolated modules.

**Status:** Passed the 1st preliminary round.

---

### 🌲 National R&D — Disaster Communication & Integrated Control
**ToBeUnicorn | System Integration / Software | 2026 - Present**

Participating in national R&D related to wildfire and landslide emergency communication systems.

Current work includes:

- Reviewing interfaces among drone relays, temporary communication nodes, field equipment, GNSS/sensors, networks, and control software
- Organizing power, communication, sensor, and equipment requirements for prototype integration
- Supporting field/system test planning
- Improving integrated-control software
- API / DB integration and functional verification
- Technical documentation and R&D evidence organization

This work strengthened my interest in **unmanned systems that must operate under real field constraints**, especially disaster-response environments.

---

## Research & Engineering Interests

My current interests are centered around:

- **Autonomous UAV / VTOL Systems**
- **Mission Autonomy**
- **Multi-UAV / Multi-Robot Systems**
- **ROS2 / PX4 / MAVLink**
- **Embedded & Edge Computing for Robotics**
- **Telemetry / Failsafe / Diagnostics**
- **UAV Communication & Networking**
- **Disaster-response Unmanned Systems**
- **Manned-Unmanned Teaming (MUM-T)**
- Aerospace mission software and system integration

I am more interested in **deployable autonomous systems** than in algorithms that remain only in simulation.

---

## Selected Projects

### 🛩️ [VTOL Autonomy Lab](https://github.com/gxmzung/vtol-autonomy-lab)

**PX4 VTOL autonomous mission verification framework**

Focus:

- MissionRaw / MAVSDK Action / Offboard / RTL responsibility separation
- Virtual FC and mission state-machine architecture
- Failsafe Supervisor
- Command Guard
- Fault-scenario verification
- FC mission upload/download consistency checks
- 100+ automated tests
- Target-estimation experiments

This project is focused on making autonomous mission logic **inspectable, testable, and failure-aware**.

---

### ✈️ [SkyEdge VTOL](https://github.com/gxmzung/skyedge_vtol)

**ROS2 / PX4-oriented UAV mission-system project**

Main themes:

- UAV mission flow
- ROS2/PX4 integration structure
- Telemetry and health monitoring
- Guidance / waypoint concepts
- Vision-assisted mission logic
- SITL-oriented verification

This repository reflects my interest in building software around a real flight stack rather than building isolated application code.

---

### ⚙️ [Mission State Machine C++](https://github.com/gxmzung/mission-state-machine-cpp)

**Autonomous mission logic and failsafe flow in C++**

Includes:

- Mission-state transitions
- Telemetry health checks
- Failsafe behavior
- Command validation
- Mission-control structure

The goal is to model autonomous behavior as explicit and testable system states.

---

### 🛠️ [FieldOps Embedded Diagnostic Suite](https://github.com/gxmzung/fieldops-embedded-diagnostic-suite)

**Embedded / field telemetry diagnostics toolkit**

Includes:

- Serial parsing
- GNSS monitoring
- Telemetry inspection
- C-based scheduling logic
- Log analysis
- Field diagnostics workflow
- Dashboard prototype

This project is based on the idea that a field system needs not only operation software, but also **diagnostic and troubleshooting tools**.

---

### 📡 [Ghost Ant Handover](https://github.com/gxmzung/ghost-ant-handover)

**UAM communication handover optimization study**

Focus:

- Network handover in mobile aerial environments
- Signal strength / latency / network-load evaluation
- Route-based handover scenarios
- Optimization-oriented decision logic
- Quantitative experiment logs

This project connects my UAV interest with **communications and mobility infrastructure**.

---

### 🌍 [RescueMap OS](https://github.com/gxmzung/rescuemap-os)

**GIS-based disaster-response software**

Focus:

- Disaster map layers
- Field information visualization
- Vulnerable-user check-in concepts
- Failure-map reporting
- Operational decision support

This project is a secondary track connecting my interest in UAVs with **disaster-response operations and spatial information**.

---

## Engineering Background

Before and during university, I have worked in environments involving both hardware and software.

### Electronics / Embedded Experience

Experience includes:

- Circuit and schematic review
- BOM management
- Gerber / PCB / SMT production workflow
- Hardware assembly and inspection
- Firmware modification and test support
- Linux / UART-based equipment
- i.MX6 / Zynq-based systems
- Production troubleshooting and technical communication

I have also participated in **aerospace/defense electronics mass-production work within externally disclosable boundaries**.

> Specific customer, subsystem, circuit, and program details are intentionally omitted from this public profile.

This background is one reason I am interested in research where software eventually has to work on **real hardware, vehicles, and field systems**.

---

## Technical Stack

### Systems / Robotics

`C` · `C++` · `Python` · `Linux` · `ROS2` · `PX4` · `MAVLink` · `MAVSDK`

### Embedded / Hardware

`UART` · `GNSS` · `Sensors` · `PCB/BOM/Gerber/SMT workflow` · `i.MX6` · `Zynq`

### Perception / Data

`OpenCV` · `YOLO` · `Kalman Filter (basic implementation)` · `Telemetry Analysis`

### Backend / Integration

`FastAPI` · `REST API` · `WebSocket` · `SQLite` · `PostgreSQL`

### Development

`Git` · `GitHub` · `Docker` · `pytest` · `GitHub Actions`

I use web/frontend technologies when they are required for **GCS, control, visualization, or system operation**, rather than as my main research direction.

---

## Selected Outcomes & Activities

- 🏆 **Grand Prize** — 2026 Future Government Innovation Idea Contest
- 🛩️ **Passed 1st Preliminary** — 24th Korea Robot Aircraft Competition
- 🌲 Participating in national R&D for wildfire/landslide emergency communication and integrated-control systems
- 📡 Conducting UAM communication handover research
- 🧪 Building and documenting UAV / embedded-system experiments on GitHub

---

## How I Work

I try to approach engineering problems in the following order:

```text
Problem
  ↓
System Boundary
  ↓
Interfaces
  ↓
Implementation
  ↓
Failure Cases
  ↓
Test
  ↓
Evidence
  ↓
Documentation
```

I value:

- clear system boundaries
- reproducible tests
- failure and fallback handling
- interface documentation
- realistic hardware constraints
- measurable results
- honest limitations

---

## Current Learning Direction

I am currently strengthening the fundamentals needed to move from a **system builder** toward an **autonomous-systems researcher**.

Current priorities include:

- Data Structures / Operating Systems / System Programming
- Robotics fundamentals
- UAV flight software
- State estimation and sensor fusion
- ROS2 / PX4 architecture
- Real-time and embedded systems
- Basic control and mathematics required for autonomous systems

My goal is not to separate theory from implementation, but to learn the theory required to **understand, modify, and validate real autonomous systems**.

---

## Long-Term Direction

```text
Embedded / Electronics
          ↓
Systems Software
          ↓
UAV / Robotics
          ↓
Mission Autonomy
          ↓
Multi-Unmanned Systems
          ↓
Autonomous Aerospace Systems
```

I want to grow into an engineer and researcher who can connect:

**hardware + embedded software + robotics + communication + mission logic + field operation**

and eventually contribute to autonomous aerospace, disaster-response, and defense systems.

---

## Contact

- GitHub: https://github.com/gxmzung
- Email: leeyj4748@naver.com
