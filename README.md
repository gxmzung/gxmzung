<div align="center">

# Lee Youngjun / 이영준

### Autonomous Systems · UAV · Embedded & Mission Software

**C / C++ · ROS2 / PX4 · MAVLink · Embedded Linux · Telemetry · GNSS / RTK · System Integration**

> I build engineering systems by connecting
> **requirements, interfaces, implementation, verification, and evidence.**

</div>

---

# About Me

I am a **Computer Engineering student and system builder** focused on autonomous, embedded, and field-deployed systems.

My engineering background began with electronics and embedded production workflows — including **PCB, BOM, Gerber, SMT, firmware testing, Linux/UART equipment, and hardware-software integration**.

Today, I am expanding that foundation into:

* UAV / VTOL mission systems
* ROS2 / PX4 / MAVLink
* embedded and mission software
* telemetry and diagnostics
* GNSS / RTK
* field communication systems
* disaster-response platforms
* AI / edge vision
* system integration and verification

I am particularly interested in systems where software must operate together with:

**flight controllers + onboard computers + sensors + communication links + networks + operators + real hardware**

```text
Requirement
    ↓
System Boundary
    ↓
Hardware / Interface
    ↓
Embedded / Communication
    ↓
Mission Logic
    ↓
Operator / GCS / Service
    ↓
Verification
    ↓
Evidence
```

My long-term direction is to grow from an engineer who can build and verify systems into a **technical project / program leader capable of understanding the systems being led**.

---

# Featured Engineering Work

## 🛩️ UAV Virtual Training / Evaluation PoC

**Software Architecture · Scenario Engine · MAVLink · Evaluation Evidence**

Designed and implemented an internal software PoC for a vendor-independent UAV training and evaluation architecture.

```text
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
```

### Implemented / Designed

* Common Drone State model
* movement-path extension
* SYSTEM / TRAINEE input separation
* generic MAVLink adapter
* decoded-stream pipeline
* live-input boundary
* 8-step internal scenario flow
* Common Training Log
* response-time evidence derivation
* rule-based evaluation adapter
* AAR Markdown generation
* Training Log / Evaluation JSON export
* requirements / ConOps / data-dictionary alignment
* automated regression testing

> **Boundary:** Internal technical PoC only.
> It is not presented as an official military requirement implementation or hardware acceptance result.

---

## 🧰 Field Gateway & Telemetry Integration

**Gateway Software · Interfaces · Field Test Preparation**

Worked on a field gateway architecture for connecting devices, positioning systems, and backend services.

### Scope

* serial auto-reconnect
* GNSS NMEA parsing
* NTRIP connection
* RTCM correction-data reception
* local buffering / resend
* backend status reporting
* CAN / RS485 / Modbus integration planning
* hardware acceptance-test preparation

```text
Field Device
    ↓
Serial / CAN / RS485
    ↓
Gateway
 ┌───────────────┐
 │ GNSS / NMEA   │
 │ NTRIP / RTCM  │
 │ Local Buffer  │
 │ Status / Log  │
 └───────────────┘
    ↓
Backend / Control System
```

---

## 📍 GNSS / RTK Integration

**Component Review · Integration Planning · Verification**

Worked on integrating GNSS / RTK components into a field gateway system.

* reviewed ZED-F9P-class GNSS / RTK components
* organized purchase items and test criteria
* designed gateway integration flow
* separated software/mock verification from hardware verification
* prepared NMEA / RTCM / RTK Fix field-test boundaries

A recurring principle in this work was to clearly distinguish:

```text
Implemented
    ≠
Simulated
    ≠
Hardware Verified
```

---

## 📡 Forest Disaster MANET / Mesh Relay

**Requirement Analysis · Technical Comparison · Test Design**

Evaluated portable MANET / Mesh relay candidates for field communication environments.

### Evaluation Factors

* NLOS communication
* multi-hop operation
* throughput
* latency
* transmission distance
* power / battery
* weight
* environmental protection
* certification
* drone-carried / deployable relay constraints

### Verification KPIs

* network deployment time
* position-update interval
* information-sharing success rate
* system availability

Supplier claims, confirmed specifications, engineering judgment, and unresolved items were tracked separately.

---

## 🛩️ VTOL Autonomous Mission Verification

[**Repository → vtol-autonomy-lab**](https://github.com/gxmzung/vtol-autonomy-lab)

PX4 VTOL mission-verification framework exploring how autonomous mission responsibilities should be separated.

### Focus

* MissionRaw / MAVSDK Action / Offboard responsibility separation
* Virtual FC
* mission state machine
* Failsafe Supervisor
* Command Guard
* fault-scenario verification
* mission consistency checks
* automated testing
* target-estimation experiments

---

# Industry R&D Experience

> Only work I personally participated in is described here.
> Company source code, credentials, customer / agency details, internal networks, and non-public requirements are intentionally excluded.

## 🌲 Disaster Integrated Control Software

**Frontend Restructuring · Integration Review · Documentation**

* analyzed an existing integrated-control frontend
* redesigned a map-centered control-room structure
* resolved React / TypeScript build and merge issues
* reviewed backend API / DB integration boundaries
* documented implementation and verification status

---

## 📶 Drone / GCS Communication Testing

**Telemetry Troubleshooting · Network Analysis · Test Planning**

* drone / controller / PC / GCS configuration review
* UDP / telemetry forwarding checks
* packet-level network troubleshooting
* external-network GPS Fix verification
* PC-side GCS connectivity boundary analysis
* acceptance-test checklist preparation

---

## 🥽 Drone Edge AI / VR Architecture

**Requirement-Gap Analysis · Data-flow Design**

Analyzed an end-to-end architecture connecting drone imagery with edge AI and XR visualization.

```text
Drone / Camera
      ↓
Edge Vision
      ↓
Detection
      ↓
Realtime Bridge
      ↓
VR / XR
```

Work included:

* HW / AI / VR requirement mapping
* interface analysis
* end-to-end data-flow design
* confirmed / unconfirmed requirement separation
* implementation-gap documentation

---

## 🎯 Precision Drop PoC

**System Concept · Requirement Review**

* analyzed drone position / altitude / velocity / release-time relationships
* reviewed required technical inputs
* organized PoC architecture
* separated known inputs, assumptions, and unresolved criteria before implementation

---

# Selected Projects

## ✈️ SkyEdge VTOL

[**Repository → skyedge_vtol**](https://github.com/gxmzung/skyedge_vtol)

ROS2 / PX4-oriented UAV mission-system project.

* UAV mission flow
* ROS2 / PX4 integration structure
* telemetry and health monitoring
* guidance / waypoint concepts
* vision-assisted mission logic
* SITL-oriented verification

**Outcome:** 24th Korea Robot Aircraft Competition — **1st Preliminary Passed**

---

## ⚙️ Mission State Machine C++

[**Repository → mission-state-machine-cpp**](https://github.com/gxmzung/mission-state-machine-cpp)

Autonomous mission and failsafe logic implemented in C++.

* explicit mission-state transitions
* telemetry health checks
* failsafe behavior
* command validation
* mission-control structure

---

## 🛠️ FieldOps Embedded Diagnostic Suite

[**Repository → fieldops-embedded-diagnostic-suite**](https://github.com/gxmzung/fieldops-embedded-diagnostic-suite)

Embedded / field telemetry diagnostic toolkit.

* serial parsing
* GNSS monitoring
* telemetry inspection
* C-based scheduling logic
* log analysis
* field diagnostic workflow
* dashboard prototype

---

## 🌍 RescueMap OS

[**Repository → rescuemap-os**](https://github.com/gxmzung/rescuemap-os)

GIS-based disaster-response software.

* disaster map layers
* field information visualization
* vulnerable-user / missing-person response concepts
* failure-map reporting
* operational decision support

---

## 📡 Ghost Ant Handover

[**Repository → ghost-ant-handover**](https://github.com/gxmzung/ghost-ant-handover)

UAM communication handover optimization study.

* aerial-network handover
* signal strength / latency / load evaluation
* route-based scenarios
* optimization-oriented decision logic
* quantitative experiment logs

---

## 🧬 BioDockLab

[**Repository → BioDockLab**](https://github.com/gxmzung/BioDockLab)

Bio AI research and experiment platform.

### Contribution

* project planning
* system architecture
* prototype development
* experiment / analysis dashboard
* API-based result integration
* technical presentation and Q&A

🏆 **Top Prize — 2026 Future Government Innovation Idea Contest**

---

## 🏫 Paejae Pick 2

[**Repository → paejae-pick-2-app**](https://github.com/gxmzung/paejae-pick-2-app)

Smart-campus student-life platform.

* service planning and development
* Flutter MVP
* campus information architecture
* department / club / cafeteria workflows
* real-device QA
* internal-test and release-scope management

🏆 **Encouragement Award — 2026 Intelligent Innovation Idea Contest**

---

# Current Projects & Competitions

| Project                   | Role / Focus                                     | Status                  |
| ------------------------- | ------------------------------------------------ | ----------------------- |
| 🛡️ **SAFE:SEARCH**       | AI Engineer · Development PM                     | Ongoing                 |
| 🚜 **AgriGuard AIoT**     | Technical PM · System Integration                | Ongoing                 |
| 🏗️ **SiteLink**          | Communication Shadow Prediction / System Concept | Competition             |
| 🚗 **MobiThread-AI**      | Digital Thread / Predictive Quality              | Research / Competition  |
| 🌍 **RescueMap OS**       | Disaster GIS                                     | Open Source Competition |
| 📡 **Ghost Ant Handover** | UAM Communication                                | UAM Olympiad            |

---

## 🛡️ SAFE:SEARCH

[**Repository → verso-team/safe-search**](https://github.com/verso-team/safe-search)

AI safety-search concept for digital-crime victims.

### Responsibilities

* development planning
* service architecture
* risk-analysis flow
* AI-result integration
* privacy / sensitive-information handling
* Human-in-the-Loop structure
* multidisciplinary team coordination

```text
Victim Input
    ↓
Sensitive Information Check
    ↓
Risk Classification
    ↓
Safe Query Generation
    ↓
Official Institution Guidance
    ↓
Confidence / Human Review
```

---

## 🚜 AgriGuard AIoT

[**Repository → agriguard-aiot**](https://github.com/PaiChai-Dev26/agriguard-aiot)

Safety platform for elderly agricultural workers combining risk prevention, fall detection, and agricultural-machine safety.

### Role

* technical scope definition
* interface boundary definition
* sensor / GPS / edge / server / web integration
* FastAPI / WebSocket real-time architecture
* hardware / API / server / UI coordination
* development checkpoint management
* demo and presentation coordination

---

# PAICHAI NEXUS

**Student-led Interdisciplinary Project Lab Initiative**

PAICHAI NEXUS is an initiative to connect students across majors through:

* real engineering problems
* multidisciplinary teams
* competitions
* research
* industry collaboration
* project-based portfolio development

```text
Problem Discovery
      ↓
Interdisciplinary Team
      ↓
Prototype
      ↓
Verification
      ↓
Competition / Research / Industry
      ↓
Portfolio
```

Current work includes project-lab planning, project discovery, team formation, and external collaboration structure design.

---

# Engineering Background

Before and during university, I worked in environments involving both hardware and software.

## Electronics / Embedded

* circuit / schematic review
* BOM management
* Gerber / PCB workflows
* SMT production
* hardware assembly and inspection
* firmware modification / testing support
* Linux / UART-based equipment
* i.MX6-based systems
* Zynq-based systems
* production troubleshooting
* cross-team technical communication

I also participated in aerospace / defense electronics production work within externally disclosable boundaries.

> Specific customers, programs, subsystems, and circuit details are intentionally omitted.

This background strongly influenced how I approach software.

I prefer software that ultimately interacts with:

**real hardware, vehicles, sensors, communication links, and field environments.**

---

# Technical Stack

## Systems / Robotics

`C` · `C++` · `Python` · `Linux`

`ROS2` · `PX4` · `MAVLink` · `MAVSDK`

---

## Embedded / Interfaces

`UART` · `CAN` · `RS485` · `Modbus`

`GNSS / RTK` · `NMEA` · `NTRIP` · `RTCM`

`i.MX6` · `Zynq`

---

## Electronics / Production

`PCB` · `BOM` · `Gerber` · `SMT`

Hardware assembly / inspection / production workflow

---

## AI / Perception / Data

`OpenCV` · `YOLO`

`Kalman Filter — basic implementation`

`Telemetry Analysis`

`RAG / LLM Prototyping`

---

## Backend / Integration

`FastAPI` · `REST API` · `WebSocket`

`Node.js` · `SQLite` · `PostgreSQL`

---

## Validation / DevOps

`Git` · `GitHub` · `Docker`

`pytest` · `Node Test Runner` · `GitHub Actions`

---

Frontend and web technologies are used primarily when required for:

* GCS
* control interfaces
* operational dashboards
* visualization
* system integration

rather than as my main engineering identity.

---

# Engineering Labs

Smaller repositories are used to strengthen low-level engineering fundamentals.

| Repository                                                                                              | Focus                           |
| ------------------------------------------------------------------------------------------------------- | ------------------------------- |
| [telemetry-packet-parser-c](https://github.com/gxmzung/telemetry-packet-parser-c)                       | C telemetry packet parsing      |
| [binary-packet-inspector-c](https://github.com/gxmzung/binary-packet-inspector-c)                       | Binary protocol inspection      |
| [uart-diagnostic-cli-c](https://github.com/gxmzung/uart-diagnostic-cli-c)                               | UART diagnostics                |
| [embedded-telemetry-lab-c](https://github.com/gxmzung/embedded-telemetry-lab-c)                         | Embedded telemetry fundamentals |
| [mission-state-machine-cpp](https://github.com/gxmzung/mission-state-machine-cpp)                       | Mission / failsafe logic        |
| [vtol-autonomy-lab](https://github.com/gxmzung/vtol-autonomy-lab)                                       | VTOL verification               |
| [px4-fault-aware-mission-verification](https://github.com/gxmzung/px4-fault-aware-mission-verification) | PX4 fault verification          |
| [ros2-px4-yaml-param-debug](https://github.com/gxmzung/ros2-px4-yaml-param-debug)                       | ROS2 / PX4 debugging            |

Some experimental repositories remain private while they contain unfinished or non-public technical context.

---

# Selected Outcomes

* 🏆 **Top Prize** — 2026 Future Government Innovation Idea Contest
* 🏆 **Encouragement Award** — 2026 Intelligent Innovation Idea Contest
* 🛩️ **1st Preliminary Passed** — 24th Korea Robot Aircraft Competition
* 🛡️ **TRAITHON — SAFE:SEARCH** — AI Engineer / Development PM
* 🚜 **National ICT Convergence AI Competition — AgriGuard AIoT** — Technical PM
* 🏗️ **LH Land Technology Competition — SiteLink**
* 🚗 **Future Mobility Industry Idea Competition — MobiThread-AI**
* 🌍 **Open Source Developer Competition — RescueMap OS**
* 📡 **UAM Olympiad — Ghost Ant Handover**
* 🌲 Industry R&D — disaster communication / integrated-control systems
* 🧭 PAICHAI NEXUS — interdisciplinary project-lab planning

---

# How I Work

My preferred engineering process is:

```text
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
```

I value:

* explicit system boundaries
* realistic hardware constraints
* reproducible testing
* failure / fallback handling
* interface documentation
* measurable evidence
* honest limitations
* clear distinction between implemented / simulated / unverified work
* communication between developers and non-developers

---

# Current Learning Direction

I am currently strengthening the fundamentals required for autonomous and embedded systems.

### Core Priorities

* Data Structures
* Operating Systems
* System Programming
* Robotics Fundamentals
* UAV Flight Software
* State Estimation / Sensor Fusion
* ROS2 / PX4 Architecture
* Real-time / Embedded Systems
* Communication / Networking
* Control and Mathematics for Autonomous Systems

My goal is not to separate theory from implementation.

I want to learn the theory required to:

**understand → modify → verify → design → lead**

real autonomous-system projects.

---

# Long-Term Direction

```text
Electronics / Embedded
        ↓
Systems & Interfaces
        ↓
UAV / Robotics / Communication
        ↓
Mission Autonomy
        ↓
Multi-Unmanned Systems
        ↓
Technical Project Leadership
        ↓
Program / System Leadership
```

My long-term interest lies in systems that combine:

**hardware + embedded software + robotics + communication + mission logic + AI + field operation**

with a particular interest in:

**autonomous aerospace, defense, and disaster-response systems.**

---

# Contact

* **GitHub:** https://github.com/gxmzung
* **Email:** [leeyj4748@naver.com](mailto:leeyj4748@naver.com)
