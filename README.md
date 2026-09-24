<div align="center">

# Youngjun Lee / 이영준

### Autonomous Systems · UAV · Embedded & Mission Software

**C / C++ · ROS2 · PX4 · MAVLink · Embedded Linux · Telemetry · GNSS / RTK · System Integration**

> I build engineering systems by connecting  
> **requirements, interfaces, implementation, verification, and evidence.**

</div>

---

## About Me

I am a **Computer Engineering student and system builder** focused on autonomous, embedded, and field-deployed systems.

My engineering background began with electronics and embedded production workflows, including:

- PCB / BOM / Gerber / SMT
- firmware testing and troubleshooting
- Linux / UART-based equipment
- i.MX6 / Zynq-based systems
- hardware-software integration

Today, my main technical interests are:

- UAV / VTOL mission systems
- ROS2 / PX4 / MAVLink
- embedded and mission software
- telemetry and diagnostics
- GNSS / RTK
- field communication systems
- disaster-response platforms
- edge AI / computer vision
- system integration and verification

I am particularly interested in systems where software must operate together with:

**flight controllers + onboard computers + sensors + communication links + networks + operators + real hardware**

<pre>
Requirement
    ↓
System Boundary
    ↓
Interfaces
    ↓
Implementation
    ↓
Verification
    ↓
Evidence
</pre>

My long-term direction is to grow from an engineer who can **build and verify systems** into a technical project / program leader who understands the systems being led.

---

## Featured Engineering Work

### 🛩️ UAV Virtual Training / Evaluation PoC

**Software Architecture · MAVLink · Scenario Engine · Evaluation Evidence**

Designed and implemented an internal software PoC for a vendor-independent UAV training and evaluation architecture.

#### Key Work

- Common Drone State model
- SYSTEM / TRAINEE input separation
- generic MAVLink adapter
- decoded-stream pipeline
- live-input boundary
- 8-step internal scenario flow
- Common Training Log
- response-time evidence derivation
- rule-based evaluation adapter
- AAR Markdown generation
- Training Log / Evaluation JSON export
- requirements / ConOps / data-dictionary alignment
- automated regression testing

<pre>
Drone / Simulator
      ↓
Generic Adapter
      ↓
Common Drone State
      ↓
Scenario Engine
      ↓
Training Log
      ↓
Evaluation Evidence
      ↓
Rule Evaluation
      ↓
AAR / Evidence Bundle
</pre>

> **Boundary:** Internal technical PoC only.  
> It is not presented as an official military requirement implementation or hardware acceptance result.

---

### 🧰 Field Gateway / GNSS / RTK Integration

**Gateway Software · Interfaces · Field Test Preparation**

Worked on field-gateway integration for connecting devices, positioning systems, and backend services.

#### Scope

- serial auto-reconnect
- GNSS NMEA parsing
- NTRIP connection
- RTCM correction-data reception
- local buffering / resend
- backend status reporting
- CAN / RS485 / Modbus integration planning
- ZED-F9P-class GNSS / RTK component review
- hardware acceptance-test preparation
- NMEA / RTCM / RTK Fix test-boundary definition

A recurring verification principle:

<pre>
Implemented
    ≠
Simulated
    ≠
Hardware Verified
</pre>

---

### 📡 Disaster Communication & Control Integration

**Network Analysis · Requirement Review · Test Design · System Integration**

Worked on communication and integrated-control systems for field and disaster-response environments.

#### Communication / Network

- MANET / Mesh relay candidate evaluation
- NLOS / multi-hop communication review
- throughput / latency analysis
- deployment-time and availability KPI definition
- drone / controller / PC / GCS configuration review
- UDP / telemetry forwarding checks
- packet-level troubleshooting
- GPS Fix / external-network verification
- acceptance-test checklist preparation

#### Control Software

- map-centered control-room frontend restructuring
- React / TypeScript build and merge troubleshooting
- backend API / DB integration-boundary review
- implementation / verification status documentation

> Company source code, credentials, customer / agency details, internal networks, and non-public requirements are intentionally excluded.

---

## Selected Projects

### ✈️ [SkyEdge VTOL](https://github.com/gxmzung/skyedge_vtol)

ROS2 / PX4-oriented UAV mission-system project.

- UAV mission flow
- ROS2 / PX4 integration structure
- telemetry and health monitoring
- guidance / waypoint concepts
- vision-assisted mission logic
- SITL-oriented verification

**Outcome:** 24th Korea Robot Aircraft Competition — **1st Preliminary Passed**

---

### ⚙️ [Mission State Machine C++](https://github.com/gxmzung/mission-state-machine-cpp)

Autonomous mission and failsafe logic implemented in C++.

- explicit mission-state transitions
- telemetry health checks
- failsafe behavior
- command validation
- mission-control structure

---

### 🛩️ [VTOL Autonomy Lab](https://github.com/gxmzung/vtol-autonomy-lab)

PX4 VTOL mission-verification framework.

- MissionRaw / MAVSDK Action / Offboard responsibility separation
- Virtual FC
- mission state machine
- Failsafe Supervisor
- Command Guard
- fault-scenario verification
- mission consistency checks
- automated testing

---

### 🛠️ [FieldOps Embedded Diagnostic Suite](https://github.com/gxmzung/fieldops-embedded-diagnostic-suite)

Embedded and field-telemetry diagnostic toolkit.

- serial parsing
- GNSS monitoring
- telemetry inspection
- C-based scheduling logic
- log analysis
- field diagnostic workflow
- dashboard prototype

---

### 📡 [Ghost Ant Handover](https://github.com/gxmzung/ghost-ant-handover)

UAM communication handover optimization study.

- aerial-network handover
- signal strength / latency / load evaluation
- route-based scenarios
- optimization-oriented decision logic
- quantitative experiment logs

---

### 🌍 [RescueMap OS](https://github.com/gxmzung/rescuemap-os)

GIS-based disaster-response software.

- disaster map layers
- field information visualization
- vulnerable-user / missing-person response concepts
- failure-map reporting
- operational decision support

---

## Interdisciplinary Projects

### 🧬 [BioDockLab](https://github.com/gxmzung/BioDockLab)

Bio AI research and experiment platform.

#### Contribution

- project planning
- system architecture
- prototype development
- experiment / analysis dashboard
- API-based result integration
- technical presentation and Q&A

🏆 **Top Prize — 2026 Future Government Innovation Idea Contest**

---

### 🏫 [Paejae Pick 2](https://github.com/gxmzung/paejae-pick-2-app)

Smart-campus student-life platform.

- service planning and development
- Flutter MVP
- campus information architecture
- department / club / cafeteria workflows
- real-device QA
- internal-test and release-scope management

🏆 **Encouragement Award — 2026 Intelligent Innovation Idea Contest**

---

## PAICHAI NEXUS

**Founder & Lab Lead · Student-led Interdisciplinary Project Lab**

PAICHAI NEXUS is a student-led interdisciplinary project organization at Pai Chai University.

My role focuses on:

- discovering project and research opportunities
- forming multidisciplinary teams
- defining project scope and expected outcomes
- coordinating technical and domain-expert collaboration
- managing schedules, responsibilities, risks, and checkpoints
- connecting development with field / user validation
- preparing research, competition, prototype, and portfolio outputs
- coordinating external collaboration with professors, companies, and institutions

> **Interdisciplinary collaboration creates value when each major contributes real domain expertise.**

<pre>
Problem Discovery
      ↓
Team Formation
      ↓
Requirement Definition
      ↓
Prototype / Research
      ↓
User / Field Validation
      ↓
Evidence
      ↓
Competition · Publication · Collaboration
</pre>

---

## Engineering Background

Before and during university, I worked in environments involving both hardware and software.

### Electronics / Embedded

- circuit / schematic review
- BOM management
- Gerber / PCB workflows
- SMT production
- hardware assembly and inspection
- firmware modification / testing support
- Linux / UART-based equipment
- i.MX6-based systems
- Zynq-based systems
- production troubleshooting
- cross-team technical communication

I also participated in aerospace / defense electronics production work within externally disclosable boundaries.

> Specific customers, programs, subsystems, and circuit details are intentionally omitted.

This background strongly influenced how I approach software.

I prefer software that ultimately interacts with:

**real hardware, vehicles, sensors, communication links, and field environments.**

---

## Technical Stack

### Systems / Robotics

`C` · `C++` · `Python` · `Linux`  
`ROS2` · `PX4` · `MAVLink` · `MAVSDK`

### Embedded / Interfaces

`UART` · `CAN` · `RS485` · `Modbus`  
`GNSS / RTK` · `NMEA` · `NTRIP` · `RTCM`  
`i.MX6` · `Zynq`

### Electronics / Production

`PCB` · `BOM` · `Gerber` · `SMT`

### AI / Perception / Data

`OpenCV` · `YOLO`  
`Kalman Filter — Basic Implementation`  
`Telemetry Analysis`  
`RAG / LLM Prototyping`

### Backend / Integration

`FastAPI` · `REST API` · `WebSocket`  
`Node.js` · `SQLite` · `PostgreSQL`

### Validation / DevOps

`Git` · `GitHub` · `Docker`  
`pytest` · `Node Test Runner` · `GitHub Actions`

> Frontend and web technologies are used primarily for GCS, control interfaces, operational dashboards, visualization, and system integration rather than as my primary engineering identity.

---

## Engineering Labs

| Repository | Focus |
| --- | --- |
| [telemetry-packet-parser-c](https://github.com/gxmzung/telemetry-packet-parser-c) | C telemetry packet parsing |
| [binary-packet-inspector-c](https://github.com/gxmzung/binary-packet-inspector-c) | Binary protocol inspection |
| [uart-diagnostic-cli-c](https://github.com/gxmzung/uart-diagnostic-cli-c) | UART diagnostics |
| [embedded-telemetry-lab-c](https://github.com/gxmzung/embedded-telemetry-lab-c) | Embedded telemetry fundamentals |
| [mission-state-machine-cpp](https://github.com/gxmzung/mission-state-machine-cpp) | Mission / failsafe logic |
| [vtol-autonomy-lab](https://github.com/gxmzung/vtol-autonomy-lab) | VTOL verification |
| [px4-fault-aware-mission-verification](https://github.com/gxmzung/px4-fault-aware-mission-verification) | PX4 fault verification |
| [ros2-px4-yaml-param-debug](https://github.com/gxmzung/ros2-px4-yaml-param-debug) | ROS2 / PX4 debugging |

---

## Selected Outcomes

- 🏆 **Top Prize** — 2026 Future Government Innovation Idea Contest
- 🏆 **Encouragement Award** — 2026 Intelligent Innovation Idea Contest
- 🛩️ **1st Preliminary Passed** — 24th Korea Robot Aircraft Competition
- 🛡️ **TRAITHON — SAFE:SEARCH** — AI Engineer / Development PM
- 🚜 **National ICT Convergence AI Competition — AgriGuard AIoT** — Technical PM
- 🏗️ **LH Land Technology Competition — SiteLink**
- 🚗 **Future Mobility Industry Idea Competition — MobiThread-AI**
- 🌍 **Open Source Developer Competition — RescueMap OS**
- 📡 **UAM Olympiad — Ghost Ant Handover**
- 🌲 **Industry R&D** — disaster communication / integrated-control systems

---

## Engineering Principles

<pre>
Problem
   ↓
Requirement
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
</pre>

I value:

- explicit system boundaries
- realistic hardware constraints
- reproducible testing
- failure / fallback handling
- interface documentation
- measurable evidence
- honest limitations
- clear distinction between implemented / simulated / unverified work
- communication between developers and non-developers

---

## Contact

- **GitHub:** https://github.com/gxmzung
- **Email:** leeyj4748@naver.com
