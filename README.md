<div align="center">

# Youngjun Lee / 이영준

### Autonomous Systems · UAV · Embedded Systems · Mission Software

**C / C++ · ROS2 · PX4 · MAVLink · Embedded Linux · GNSS / RTK · Telemetry · System Integration**

I build and verify engineering systems that connect  
**software, hardware, communication, autonomy, and real-world operation.**

</div>

---

# About

I am **Youngjun Lee (이영준)**, a Computer Engineering student at **Pai Chai University (배재대학교)** focused on autonomous, embedded, and field-deployed systems.

My background spans:

- electronics and embedded production
- circuit / PCB workflows
- Linux / UART-based equipment
- UAV / GCS telemetry
- GNSS / RTK
- mission software
- field communication
- disaster-response systems
- hardware-software integration
- interdisciplinary technical project leadership

In **2023**, I contributed to circuit design for production hardware related to the **KF-21 AESA radar**, within a limited and externally disclosable scope.

I currently participate in field-oriented R&D and systems-integration work at **ToBeUnicorn**, involving disaster-response platforms, UAV/GCS integration, GNSS/RTK, communication systems, operational dashboards, and technical verification.

### Primary Direction

**Embedded Systems → UAV / Robotics → Mission Autonomy → System Integration → Technical Program Leadership**

> **Implemented ≠ Simulated ≠ Hardware Verified**
>
> I try to make this boundary explicit in implementation, testing, and documentation.

---

---

# At a Glance

| Area | Current Focus |
| --- | --- |
| **Industry R&D** | Disaster-response integrated control · UAV/GCS · GNSS/RTK · Field gateway · Technical verification |
| **Autonomous Systems** | ROS2 · PX4 · MAVLink · VTOL mission software · Failsafe / verification |
| **University R&D** | Smart ICT Makerthon · GIS academic research · Smart-campus / mobility · Smart agriculture |
| **Leadership** | Founder & Lab Lead, PAICHAI NEXUS · Technical PM / interdisciplinary coordination |
| **Selected Results** | BioDockLab 1st Place · Paejae Pick Encouragement Award · Robot Aircraft Competition 1st Preliminary Passed |

---

# Featured Engineering Work

| Work | Focus |
| --- | --- |
| **UAV Training / Evaluation PoC** | Common drone state · MAVLink adapter · scenario engine · evaluation evidence · AAR |
| **Field Gateway / GNSS / RTK** | NMEA · NTRIP · RTCM · buffering · backend status · field verification |
| **Disaster Response Platform** | Integrated control UI · UAV/GCS · positioning · maps · communications · acceptance testing |

---

<details>
<summary><strong>🛩️ UAV Training / Evaluation PoC</strong></summary>

**Type:** Industry R&D / Internal Technical PoC  
**Project / Work:** Vendor-Independent UAV Training & Evaluation Architecture  
**Role:** Software Architecture · MAVLink Integration · Scenario Engine · Evaluation Evidence

### Problem / Objective

Different UAVs and simulators expose different telemetry and control interfaces. The PoC explores how those inputs can be normalized into a common state model and then used for repeatable scenario execution, logging, evaluation, and after-action review.

### Development / Engineering

- Common Drone State model
- SYSTEM / TRAINEE input separation
- generic MAVLink adapter
- decoded-stream pipeline
- live-input boundary
- internal scenario flow
- Common Training Log
- response-time evidence derivation
- rule-based evaluation adapter
- AAR Markdown generation
- Training Log / Evaluation JSON export
- requirements / ConOps / data-dictionary alignment
- automated regression testing

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

### Verification

The architecture is designed so that scenario execution and evaluation evidence can be reproduced from logged inputs rather than depending only on operator interpretation.

**Status:** Internal Technical PoC

> It is not presented as an official military requirement implementation or hardware acceptance result.

</details>

---

<details>
<summary><strong>🧰 Field Gateway / GNSS / RTK Integration</strong></summary>

**Type:** Industry R&D  
**Project / Work:** Field Gateway & Positioning Integration  
**Role:** Gateway Software · GNSS/RTK Interfaces · Backend Integration · Field-Test Preparation

### Problem / Objective

Field equipment produces useful data only when device connectivity, positioning validity, correction data, buffering, and backend reporting continue to work together under unstable field conditions.

The work therefore focuses on making positioning and device data operationally usable rather than treating GNSS, RTK, serial links, and backend APIs as isolated components.

### Development / Engineering

- serial auto-reconnect
- GNSS NMEA parsing
- NTRIP client connection
- RTCM correction-data reception
- local buffering / resend
- backend status reporting
- persisted RTK-position integration
- invalid / unavailable Fix filtering
- zero-coordinate filtering
- freshness / signal-quality handling
- ZED-F9P-class GNSS / RTK component review
- CAN / RS485 / Modbus integration planning
- hardware acceptance-test preparation
- NMEA / RTCM / RTK Fix test-boundary definition

### Validation Focus

```text
Message Received
      ↓
Parsed Correctly
      ↓
Position Valid
      ↓
RTK / Fix State Valid
      ↓
Backend Reflected
      ↓
Operational UI Visible
      ↓
Hardware / Field Verified
```

Receiving an NMEA or RTCM message does not by itself prove valid positioning or field readiness.

**Status:** Ongoing / Field Integration

</details>

---

<details>
<summary><strong>🌲 Disaster Response Platform & Integrated Control</strong></summary>

**Type:** Industry R&D  
**Project / Work:** Wildfire / Landslide Integrated Control Platform  
**Role:** System Integration · Control-Room Software · UAV/GCS · GNSS/RTK · Technical Verification

### Problem / Objective

The project connects disaster-response operations with mapping, UAV telemetry, positioning, field communications, backend services, and operational software.

The engineering challenge is not merely displaying data, but making multiple devices and services behave as one system under field constraints.

### Development / Engineering

- map-centered integrated-control UI restructuring
- wildfire / landslide operational map layers
- UAV / GCS telemetry integration
- GNSS / RTK position handling
- live vehicle / device marker visualization
- persisted RTK-position exposure to dashboards
- maintaining live markers during delayed database updates
- alert / event display integration
- terrain-analysis visualization
- LAN-based operational communication / chat integration
- backend API / database integration-boundary review
- telemetry-forwarding checks
- packet-level troubleshooting
- GPS Fix / external-network verification
- deployment / availability KPI review
- field-test and acceptance-test checklist preparation
- implementation / simulation / hardware-verification status documentation

### Verification Principle

Implementation status is separated into:

- implemented
- simulated
- live-input verified
- field-tested
- hardware-verified
- not yet verified

This avoids presenting software implementation as field-proven before the required device or field validation is complete.

**Status:** Ongoing Industry R&D

> Company source code, credentials, customer / agency details, internal networks, and non-public requirements are intentionally excluded.

---

</details>

---

# Selected Engineering Projects

---

<details>
<summary><strong>✈️ SkyEdge VTOL</strong></summary>

**Type:** Autonomous UAV Project / Competition  
**Project:** [SkyEdge VTOL](https://github.com/gxmzung/skyedge_vtol)  
**Role:** Mission-System Development · Integration

### Development / Engineering

- UAV mission flow
- ROS2 / PX4 integration
- telemetry and health monitoring
- guidance / waypoint concepts
- vision-assisted mission logic
- SITL-oriented verification
- RTK-GNSS integration concepts
- onboard-computing integration

**Tech:** ROS2 · PX4 · MAVLink · VTOL · Telemetry · Computer Vision  
**Result:** 24th Korea Robot Aircraft Competition — **1st Preliminary Passed**

---

</details>

---

<details>
<summary><strong>⚙️ Mission State Machine C++</strong></summary>

**Type:** Engineering Lab / Mission Software  
**Project:** [Mission State Machine C++](https://github.com/gxmzung/mission-state-machine-cpp)  
**Role:** C++ Mission / Failsafe Logic Development

### Development / Engineering

- explicit mission-state transitions
- telemetry health checks
- failsafe behavior
- command validation
- mission-control structure

**Tech:** C++ · State Machine · Mission Logic · Failsafe · Embedded Systems

---

</details>

---

<details>
<summary><strong>🛩️ VTOL Autonomy Lab</strong></summary>

**Type:** Engineering Lab / Verification  
**Project:** [VTOL Autonomy Lab](https://github.com/gxmzung/vtol-autonomy-lab)  
**Role:** PX4 Mission Verification Framework Development

### Development / Engineering

- MissionRaw / MAVSDK Action / Offboard responsibility separation
- Virtual FC
- mission state machine
- Failsafe Supervisor
- Command Guard
- fault-scenario verification
- mission consistency checks
- automated testing

**Tech:** PX4 · MAVSDK · VTOL · Autonomous Mission · Verification

---

</details>

---

<details>
<summary><strong>🛠️ FieldOps Embedded Diagnostic Suite</strong></summary>

**Type:** Engineering Lab / Field Diagnostics  
**Project:** [FieldOps Embedded Diagnostic Suite](https://github.com/gxmzung/fieldops-embedded-diagnostic-suite)  
**Role:** Embedded / Telemetry Diagnostic Tool Development

### Development / Engineering

- serial parsing
- GNSS monitoring
- telemetry inspection
- C-based scheduling logic
- log analysis
- field diagnostic workflow
- dashboard prototype

**Tech:** Embedded · C · Serial · GNSS · Telemetry · Diagnostics

---

</details>

---

<details>
<summary><strong>📡 Ghost Ant Handover</strong></summary>

**Type:** UAM Communication Research / Competition  
**Project:** [Ghost Ant Handover](https://github.com/gxmzung/ghost-ant-handover)  
**Role:** Handover Logic / Experiment Design

### Development / Research

- aerial-network handover
- signal-strength evaluation
- latency / network-load comparison
- route-based scenarios
- optimization-oriented decision logic
- quantitative experiment logs

**Tech:** UAM · Networking · Handover · Optimization

---

</details>

---

<details>
<summary><strong>🌍 RescueMap OS</strong></summary>

**Type:** Open Source / Disaster Response / Competition  
**Project:** [RescueMap OS](https://github.com/gxmzung/rescuemap-os)  
**Role:** GIS Service Planning · Development

### Development / Engineering

- disaster map layers
- field-information visualization
- vulnerable-user / missing-person response concepts
- failure-map reporting
- operational decision support
- map-centered incident awareness

**Tech:** GIS · Disaster Response · Mapping · Decision Support

---

</details>

---

# Technical Journey

---

<details>
<summary><strong>2010–Present · Full Technical Journey</strong></summary>

## 2010–2018 · Foundations & Early Mentorship

**Stage:** Early Technical Foundation

### Learning / Exploration

- computer architecture
- low-level data processing
- embedded logic
- hardware-software interaction
- communication / IoT concepts
- firmware and system-security fundamentals
- control and autonomous-system concepts

This period shaped my interest in systems where software interacts directly with hardware and physical environments.

---

## 2019–2021 · Technical Exploration & Direction Setting

**Stage:** High School / Technical Exploration

### Learning / Exploration

- low-level system behavior
- hardware-software interfaces
- embedded / real-time systems
- communication
- control
- system architecture

This period helped define the direction that later led me toward embedded engineering, defense systems, UAVs, and autonomous systems.

---

## 2022–2024 · Defense & Embedded Engineering

**Stage:** Electronics / Embedded Production & Defense-Related Engineering

### Engineering Experience

- circuit / schematic review
- PCB / BOM / Gerber / SMT
- firmware testing and troubleshooting
- Linux / UART-based equipment
- i.MX6 / Zynq-class systems
- production troubleshooting
- hardware-software integration
- cross-team technical communication

In **2023**, I contributed to circuit design for production hardware related to the **KF-21 AESA radar**, within externally disclosable boundaries.

> This refers only to my limited engineering contribution and does not imply responsibility for the overall radar, aircraft, or subsystem design.

---

## 2025 · Reframing the Technical Path

**Stage:** Technical Direction Setting

### Direction

**Embedded Systems → UAV / Robotics → Mission Software → System Integration**

I also became increasingly interested in connecting practical engineering experience with university education, interdisciplinary teams, and project leadership.

---

## 2026–Present · University × Industry × R&D

**Stage:** Computer Engineering Student · Industry R&D · Project Leadership

### Current Work

- UAV / GCS / GNSS / RTK integration
- disaster-response and field communication systems
- autonomous mission software
- technical documentation and test preparation
- Founder & Lab Lead of **PAICHAI NEXUS**
- maker / hackathon / competition projects
- academic conference research
- campus technical collaboration
- interdisciplinary project leadership

**Working Principle:** build → verify → integrate → lead

---

</details>

---

# University Competitions, Hackathons & Academic Activities

| Program / Competition | Project | Result / Status |
| --- | --- | --- |
| Future Government Innovation Idea Contest | **BioDockLab** | 🏆 Top Prize / 1st Place |
| Intelligent Innovation Idea Contest | **Paejae Pick** | 🏆 Encouragement Award |
| 24th Korea Robot Aircraft Competition | **SkyEdge VTOL** | 1st Preliminary Passed |
| National ICT Convergence AI Competition | **AgriGuard AIoT** | Competition Project |
| TRAITHON | **SAFE:SEARCH** | Competition Project |
| 17th LH Land Technology Competition | **SiteLink** | Proposal / Prototype |
| Future Mobility Industry Idea Competition | **MobiThread-AI** | Research / Competition |
| UAM Olympiad | **Ghost Ant Handover** | Research / Competition |
| Open Source Developer Competition | **RescueMap OS** | Open Source / Competition |
| 2026 Smart ICT Makerthon | **NEXUS NEST** | Field Validation Planned |
| 2026 Smart ICT Convergence Academic Conference | **Pai Chai–Mokwon GIS Route Research** | Paper / Poster / Presentation |
| Regional Social Venture Hackathon | **PAICHAI NEXUS** | ✅ Participation Confirmed |
| PCU Presentation Competition | Engineering / Project Storytelling | Preparing |

---

<details>
<summary><strong>🏆 2026 Future Government Innovation Idea Contest</strong></summary>

**Type:** Idea / Innovation Competition  
**Project:** BioDockLab  
**Role:** Project Planning · System Architecture · Prototype Development

### Development / Engineering

- Bio AI research / experiment platform
- experiment and analysis dashboard
- API-based result integration
- prototype development
- interactive exhibition prototype
- technical presentation and Q&A

**Result:** 🏆 **Top Prize / 1st Place**

---

</details>

---

<details>
<summary><strong>🏆 2026 Intelligent Innovation Idea Contest</strong></summary>

**Type:** University Innovation Competition  
**Project:** Paejae Pick  
**Role:** Service Planning · Development · QA

### Development / Engineering

- smart-campus mobile service
- Flutter MVP
- campus information architecture
- department / club / cafeteria workflows
- real-device QA
- release-scope management
- future mobility-service expansion concepts

**Result:** 🏆 **Encouragement Award**

---

</details>

---

<details>
<summary><strong>🛩️ 24th Korea Robot Aircraft Competition</strong></summary>

**Type:** National UAV / Robotics Competition  
**Project:** SkyEdge VTOL  
**Role:** Mission-System Development · Integration

### Development / Engineering

- ROS2 / PX4 integration
- Pixhawk-based flight-control integration
- autonomous mission logic
- telemetry and health monitoring
- RTK-GNSS
- onboard computing
- computer vision
- mission-system verification

**Result:** **1st Preliminary Passed**

---

</details>

---

<details>
<summary><strong>🚜 National ICT Convergence AI Competition</strong></summary>

**Type:** National AI / ICT Convergence Competition  
**Project:** AgriGuard AIoT  
**Role:** Technical PM · System Integration

### Problem / Objective

AgriGuard AIoT is an agricultural-environment safety platform that combines field sensors, positioning, edge devices, server communication, and real-time monitoring.

The main engineering task is coordinating multiple layers so that device data is collected, transferred, processed, and presented consistently.

### Development / Engineering

- sensor integration
- GPS / position handling
- edge-device integration
- FastAPI backend
- WebSocket-based real-time communication
- server / API integration
- monitoring UI coordination
- hardware / API / server / UI interface definition
- development checkpoint management
- multidisciplinary development coordination

### Role Focus

As Technical PM / System Integration, the work focuses on ensuring that each technical component connects to the next layer through clear interfaces, ownership, and checkpoints.

**Status:** Competition Project / Development

</details>

---

<details>
<summary><strong>🛡️ TRAITHON</strong></summary>

**Type:** AI / Digital Safety Competition  
**Project:** SAFE:SEARCH  
**Role:** AI Engineer · Development PM

### Problem / Objective

SAFE:SEARCH is an AI-assisted safety-search platform intended to support victims of digital crime while minimizing unnecessary exposure of sensitive information.

### Development / Engineering

- development planning
- service architecture
- AI-result integration
- safety-search workflow
- privacy / sensitive-information handling
- Human-in-the-Loop review design
- multidisciplinary team coordination
- development milestone management
- result-review / escalation concepts

### Design Principle

```text
AI Search / Analysis
      ↓
Candidate Result
      ↓
Human Review
      ↓
Confirmed Action / Guidance
```

AI output is treated as decision support rather than an unquestioned final judgment.

**Status:** Competition Project / Development

</details>

---

<details>
<summary><strong>🏗️ 17th LH Land Technology Competition</strong></summary>

**Type:** Construction / Infrastructure Technology Competition  
**Project:** SiteLink — Construction-Site Wi-Fi Placement Optimization for Changing Work Phases  
**Role:** System Planning · Communication Coverage Analysis · Prototype Design

### Problem

Temporary Wi-Fi / AP layouts at construction sites are often planned for an early construction phase and then remain fixed even as walls, structures, work zones, safety facilities, and equipment locations change.

This can create:

- communication-shadow areas
- reduced coverage in high-priority work zones
- inefficient AP relocation
- unnecessary additional AP installation
- repeated manual site surveys after construction-stage changes

### Development / Engineering

SiteLink was proposed as a decision-support system that uses **CAD / BIM-based spatial information** and communication-coverage analysis to recommend AP relocation after site-layout changes.

Core functions include:

- CAD / BIM spatial-data input
- construction-stage before / after comparison
- AP position and communication-coverage visualization
- communication-shadow prediction
- high-priority zone definition
- candidate AP-position generation
- automatic comparison of relocation candidates
- AP relocation-distance calculation
- new-AP addition minimization
- before / after coverage comparison
- field-console visualization

### Priority-Area Evaluation

Rather than optimizing only total site coverage, SiteLink can assign higher importance to operationally critical areas such as:

- CCTV / IoT sensor zones
- worker-concentration zones
- safety-management areas
- material / equipment routes
- emergency-access areas
- areas where reliable field communication is especially important

### Prototype Result

In the proposal's simplified two-phase construction scenario:

- total analyzed-area coverage: **45.2% → 45.5%**
- priority-area coverage: **76.0% → 79.1%**
- improvement in priority-area coverage: **+3.1%p**
- one existing AP was moved by approximately **6.3 m**
- **no new AP** was added
- **45 candidate positions** were automatically compared

The objective was not to maximize coverage at any cost, but to find a practical relocation option that improves important work-zone coverage while minimizing equipment movement and additional installation.

### Field Application Concept

A future deployment workflow would be:

1. import CAD / BIM site layout
2. define the current construction phase
3. measure or estimate existing AP coverage
4. identify communication-shadow / priority areas
5. generate AP relocation candidates
6. compare coverage, movement distance, and equipment cost
7. select a practical relocation plan
8. update the model as the construction phase changes

**Status:** Competition Proposal / Prototype Concept

---

</details>

---

<details>
<summary><strong>🏗️ SiteLink</strong></summary>

**Type:** Construction-Site Communication / Infrastructure Optimization  
**Project:** SiteLink  
**Role:** System Planning · Coverage Analysis · Prototype Design

### Development / Engineering

- CAD / BIM-based construction-space interpretation
- changing construction-stage comparison
- AP coverage visualization
- communication-shadow detection
- priority-zone weighting
- candidate AP relocation analysis
- movement-distance / new-AP minimization
- before / after coverage comparison

**Prototype Result:** Priority-area coverage improved from **76.0% to 79.1%** in the proposal scenario while moving one AP approximately **6.3 m** and adding no new AP.

---

</details>

---

<details>
<summary><strong>🚗 Future Mobility Industry Idea Competition</strong></summary>

**Type:** Future Mobility / Industry Competition  
**Project:** MobiThread-AI  
**Role:** Research Planning · Engineering-System Concept Design

### Problem / Objective

MobiThread-AI explores how fragmented engineering and lifecycle data can be connected through a Digital Thread so that quality issues and engineering changes can be traced across the mobility-product lifecycle.

### Development / Research

- Digital Thread concept
- engineering-data integration
- lifecycle information linkage
- predictive-quality concept
- AI-assisted engineering analysis
- traceability of engineering changes
- manufacturing / quality / lifecycle data connection
- decision-support concept for mobility engineering

```text
Design Data
   ↓
Manufacturing Data
   ↓
Quality Data
   ↓
Operational / Lifecycle Data
   ↓
AI-Assisted Analysis & Traceability
```

**Status:** Research / Competition Project

</details>

---

<details>
<summary><strong>📡 UAM Olympiad</strong></summary>

**Type:** UAM / Communication Competition  
**Project:** Ghost Ant Handover  
**Role:** Handover Logic · Scenario / Experiment Design

### Problem / Objective

Aerial mobility platforms move through communication environments where the strongest signal at one instant is not always the best long-term link.

Ghost Ant Handover studies how handover decisions can consider multiple variables rather than relying only on instantaneous signal strength.

### Development / Research

- aerial-network handover model
- signal-strength comparison
- latency evaluation
- network-load evaluation
- route-based communication scenarios
- optimization-oriented decision logic
- quantitative experiment logs
- handover-condition comparison

```text
Signal Strength
      +
Latency
      +
Network Load
      +
Route Context
      ↓
Handover Decision
```

**Status:** Research / Competition Project

</details>

---

<details>
<summary><strong>🌍 Open Source Developer Competition</strong></summary>

**Type:** Open Source / Disaster Response Competition  
**Project:** RescueMap OS  
**Role:** GIS Service Planning · Development

### Problem / Objective

Disaster response often requires multiple kinds of field information to be understood spatially and quickly.

RescueMap OS organizes incident, field, and vulnerable-user information around a map-centered operational interface.

### Development / Engineering

- disaster map layers
- field-information visualization
- vulnerable-user / missing-person response concepts
- incident / failure-map reporting
- operational decision-support UI
- location-centered information organization
- map-based situation awareness

### Product Direction

The system is designed so that an operator can understand **where** an issue exists, **what** is happening there, and **what information is needed next** from the same map context.

**Status:** Open Source / Competition Project

</details>

---

<details>
<summary><strong>🔧 2026 Smart ICT Makerthon</strong></summary>

**Type:** University Makerthon  
**Project:** NEXUS NEST — AI-Based Kindergarten Classroom Spatial-Safety Diagnostic Service  
**Field:** Early Childhood Education × Computer Engineering × Game Engineering × Architecture  
**Role:** Project Direction · System Planning · Interdisciplinary Coordination

### Problem / Objective

NEXUS NEST starts from real classroom-operation problems rather than selecting technology first.

The goal is to help teachers review classroom space, safety, and facility conditions by connecting actual classroom constraints with an ICT prototype.

### Service Flow

```text
Classroom Material
(Photo / Floor Plan)
        ↓
Risk Candidates
        ↓
Possible Layout Changes
        ↓
3D Before / After Comparison
        ↓
Teacher Review
```

### First Prototype — Risk Categories

- **collision risk:** obstacles or furniture at child eye / movement level
- **movement risk:** narrow passages and circulation conflicts
- **observation blind spots:** spaces blocked from a teacher's line of sight
- **evacuation obstruction:** furniture blocking entrances or evacuation routes

### Development / Validation

- classroom photo / floor-plan input
- spatial-risk candidate visualization
- possible furniture-layout alternatives
- 3D before / after comparison
- teacher feedback loop
- repeated prototype revision based on field conditions

### Field Testbed

A Pai Chai University-affiliated kindergarten is proposed as the first testbed.

Initial validation focuses on:

- teacher interviews
- empty-classroom inspection
- furniture / passage / entrance / blind-spot review
- classroom floor-plan or non-identifiable photo use
- prototype usability review
- checklist-based field inspection

The initial test intentionally avoids:

- recording children
- child voice collection
- CCTV video
- child behavior / emotion analysis
- permanent facility changes
- continuous equipment installation

### Validation Criteria

- field validity / safety usefulness
- spatial feasibility of suggested layouts
- understandability and user burden
- willingness to reuse the system

**Status:** Preparing / Field Validation Planned

</details>

---

<details>
<summary><strong>📚 2026 Smart ICT Convergence Academic Conference</strong></summary>

**Type:** Academic Conference  
**Research Project:** GIS-Based Comparative Analysis of Underground Connection Route Alternatives between Pai Chai University and Mokwon University under a Hypothetical Integrated-Campus Scenario  
**Role:** Research Planning · GIS Analysis · Route Comparison · Paper / Poster Preparation

### Research Objective

Inspired by the universities' 2023 integrated-education discussions, the study defines a hypothetical dual-campus operation scenario around 2033 and compares three underground connection-route alternatives between Pai Chai University and Mokwon University.

The study is intended as a **preliminary spatial comparison**, not as proof of constructability, structural safety, settlement behavior, or final engineering feasibility.

### Data / Method

- NASA SRTM Global 1 arc-second elevation data (~30 m)
- OpenStreetMap building / road / campus-boundary data
- EPSG:5186 spatial integration
- 20 m computational grid
- 8-direction Dijkstra route search
- conceptual longitudinal-profile comparison
- building-footprint intersection analysis
- 30 m spatial screening-buffer comparison

Three candidate routes were generated using different priorities:

- **Route A:** direct / shortest-distance baseline
- **Route B:** reduced slope and building proximity
- **Route C:** road-corridor preference added to route generation

### Quantitative Comparison

- Route A: **2,027 m**
- Route B: **2,299 m**
- Route C: **2,271 m**
- mean bored-section cover: **38 m / 38 m / 31 m**
- building-footprint intersections: **0 / 0 / 1**
- buildings within 30 m screening buffer: **6 / 0 / 3**

### Findings

- Route A provides the strongest distance efficiency.
- Route B minimizes building proximity and can be considered when reduced interaction with surrounding buildings is prioritized.
- Route C has the lowest mean cover but is longer than Route A and intersects one building footprint.
- No single route dominates every indicator.
- Route A and Route B are therefore reasonable candidates for further investigation depending on the evaluation priority.

### Research Limitations

The analysis is limited by:

- SRTM source resolution
- OpenStreetMap completeness
- lack of geological / borehole investigation data
- conceptual longitudinal-profile assumptions
- fixed spatial screening buffer

Further work would require detailed surveying, geotechnical investigation, section design, ventilation, disaster prevention, demand, and cost analysis.

### Deliverables

- 4-page academic paper
- research poster
- presentation

The draft was reviewed by **Prof. Hoe-Kyung Jung (정회경)**, and no additional revisions were requested at that review stage.

**Status:** Paper / Poster / Presentation Preparation

---

</details>

---

<details>
<summary><strong>🤝 2026 Regional Community Problem-Solving Innovative Social Venture Hackathon</strong></summary>

**Type:** Regional University Social Venture Hackathon  
**Team:** PAICHAI NEXUS  
**Team Structure:** 5-person interdisciplinary team  
**Fields:** Computer Engineering · Software · IT Management · Architecture  
**Role:** Team Lead · Interdisciplinary Project Coordination

### Program / Development Direction

- real community problem discovery
- interdisciplinary problem definition
- rapid solution concept development
- prototype / service-model design
- validation
- social-impact framing

### Participation

- NEXUS application submitted as a five-member interdisciplinary team
- participation confirmation received
- regional program involving **13 universities in the Daejeon area**
- up to **two teams per university**

**Status:** ✅ Participation Confirmed

---

</details>

---

<details>
<summary><strong>🎤 PCU Presentation Competition</strong></summary>

**Type:** University Presentation Competition  
**Project / Topic:** Engineering Projects & Technical Storytelling  
**Role:** Presentation Planning · Technical Communication

### Preparation

- evidence-based explanation
- presentation structure
- project storytelling
- technical-to-nontechnical communication
- project experience visualization

**Status:** Preparing

---

</details>

---

# University Programs & Campus Collaboration

---

<details>
<summary><strong>🎓 2026 NASEOM Competency Maker</strong></summary>

**Type:** University Maker Program  
**Project:** Paejae Pick 2.0  
**Role:** Development Lead · Project Coordination

### Development / Engineering

The selected project expands Paejae Pick from a campus-life service toward a smart-campus / future-mobility platform.

- integrated campus services
- 3D indoor navigation
- mobile-device testing
- campus route / destination interaction
- autonomous shuttle call / status concepts
- autonomous delivery call / status concepts
- ROS2-connected mobility-service direction
- future-mobility screen design

### Validation / Operation

Because the project is intended for actual student use, device compatibility and real-device testing are treated as part of development rather than as a final optional step.

**Status:** ✅ Selected Project

</details>

---

<details>
<summary><strong>🤝 NEXUS × College of Business Administration</strong></summary>

**Type:** University Collaboration / Event Technical Support  
**Project:** 2026 College of Business Administration Academic Festival Support  
**Role:** Technical Coordination · Event-System Development · Design / Media Collaboration

### Problem / Objective

The collaboration supports a real university academic festival by integrating design, promotion, audience participation, and event-operation technology instead of treating each output as a separate task.

### Development / Production

- event poster design and production
- promotional video production
- QR-based on-site audience voting
- audience-evaluation flow design
- event information / participation flow
- event-system development
- technical support
- organizer / designer / developer coordination

### Event Context

The festival includes:

- invited company sessions
- CEO special lecture
- academic competition finals
- audience evaluation
- awards / on-site participation programs

The technical collaboration supports both visible promotional materials and the operational flow behind the event.

**Status:** Ongoing Collaboration

---

</details>

---

# Interdisciplinary Projects

| Project | Domain | Current Direction |
| --- | --- | --- |
| **BioDockLab** | Bio AI | Research / experiment platform · interactive prototype |
| **Paejae Pick 2.0** | Smart Campus / Mobility | Mobile app · indoor navigation · autonomous mobility |
| **Smart Seedling AI** | Agriculture / Vision AI / IoT | Stress detection · greenhouse sensing · integrated control |
| **Healthcare HIS** | Healthcare IT | Nursing workflow · information architecture |
| **Underground Connection Route GIS Research** | GIS / Smart Construction | Candidate-route comparison · spatial screening |
| **NEXUS NEST** | Early Childhood / Spatial Safety | Classroom risk review · 3D layout comparison · teacher validation |

---

<details>
<summary><strong>🧬 BioDockLab</strong></summary>

**Type:** Bio AI / Research & Experiment Platform  
**Project:** [BioDockLab](https://github.com/gxmzung/BioDockLab)  
**Role:** Project Planning · System Architecture · Prototype Development · Technical Presentation

### Problem / Objective

BioDockLab was designed as a platform concept that makes biological research data and analysis workflows easier to explore, demonstrate, and connect through a single interactive environment.

The project focused on turning a difficult-to-understand research workflow into a prototype that could be operated and explained directly at an exhibition booth.

### Development / Engineering

- project / service planning
- system architecture
- Raspberry Pi-based exhibition prototype
- 7-inch touch display interface
- Raspberry Pi Camera integration
- LED ring / button interaction
- sample / image workflow
- capture / analyze API flow
- experiment / analysis dashboard
- API-based result integration
- biological data-source linkage concepts
- interactive exhibition UI
- hardware / software integration
- technical presentation and Q&A

### Prototype / Demonstration

```text
Sample / Image
      ↓
Camera Capture
      ↓
Analysis Request
      ↓
Result Visualization
      ↓
User Interaction / Explanation
```

The system included API flows for health checks, sample handling, image capture, analysis, LED control, and debugging.

### Validation / Outcome

- operated as an interactive experience booth
- demonstrated to university visitors and stakeholders
- used a working prototype rather than a slide-only concept

**Result:** 🏆 **2026 Future Government Innovation Idea Contest — Top Prize / 1st Place**

</details>

---

<details>
<summary><strong>🏫 Paejae Pick 2.0</strong></summary>

**Type:** Smart Campus / Mobility Platform  
**Project:** [Paejae Pick 2.0](https://github.com/gxmzung/paejae-pick-2-app)  
**Role:** Development Lead · Service Planning · Mobile QA · System Expansion Planning

### Problem / Objective

Paejae Pick began as a campus-life platform intended to reduce fragmentation between student information, campus services, departments, clubs, food services, and mobility-related functions.

The 2.0 direction expands the project from a student-life app into a broader smart-campus interface.

### Development / Engineering

- Flutter-based mobile MVP
- campus information architecture
- department / club / cafeteria service flows
- real-device QA
- internal-test and release-scope management
- mobile-device compatibility review
- 3D indoor-map / navigation concept
- campus route and destination UI
- autonomous shuttle / delivery-service call concepts
- vehicle / robot status-display concepts
- ROS2-connected mobility-service direction
- future smart-mobility screen design

```text
Campus Information
      +
Indoor Navigation
      +
Student Services
      +
Autonomous Mobility
      ↓
Integrated Smart-Campus App
```

### Validation / Outcome

- mobile MVP and real-device testing
- continued redesign toward smart-campus / future-mobility integration

**Results:**
- 🏆 **2026 Intelligent Innovation Idea Contest — Encouragement Award**
- 🎓 **2026 NASEOM Competency Maker — Selected Project**

</details>

---

<details>
<summary><strong>🌱 Smart Seedling AI / AI Farmer</strong></summary>

**Type:** Smart Agriculture / Vision AI / IoT / ROS2  
**Project:** [Smart Seedling AI](https://github.com/paichai-nexus/smart-seedling-ai)  
**Role:** Project Coordination · System Integration · Research Planning  
**Team Direction:** Horticulture × Computer Engineering × Electronics × UAV / Robotics × Spatial / Greenhouse Design

### Problem / Objective

Smart Seedling AI is being developed as a greenhouse research and prototyping platform that combines **crop imagery, thermal information, environmental sensing, and field automation**.

The goal is not to stop at monitoring. The longer-term direction is an **AI Farmer closed-loop system** that repeatedly:

```text
Crop / Environment Sensing
          ↓
Vision + Sensor Data Fusion
          ↓
Stress / Growth Diagnosis
          ↓
AI-Assisted Decision
          ↓
Irrigation / Ventilation / Shading / Treatment
          ↓
Re-measurement & Feedback
          ↓
Data Accumulation / Model Improvement
```

### Research Axis 1 — Multimodal Stress & Growth Diagnosis

The first research axis combines multiple observation channels so that crop abnormalities can be detected earlier and interpreted with environmental context.

Planned / reviewed inputs include:

- fixed RGB camera imagery
- thermal-camera imagery
- thermal-drone imagery for wider-area inspection
- greenhouse temperature / humidity
- soil moisture
- illuminance
- EC
- pH

Target outputs include:

- water-stress detection
- heat-stress detection
- crop-growth anomaly detection
- risk-location visualization
- probable-cause candidates
- greenhouse monitoring / control dashboard

Rather than treating a thermal image or a sensor threshold as proof by itself, the project aims to compare **visual symptoms + thermal response + environmental measurements** together.

### Research Axis 2 — Long-Term Crop Dataset & Diagnostic Model

A primary crop is planned to be selected and observed continuously so that the project can build a crop-specific dataset rather than relying only on one-time demonstration data.

Long-term data categories include:

- normal growth
- water stress
- heat stress
- pests / disease
- nutrient disorders

The research direction is to connect:

```text
Individual / Zone ID
      +
RGB / Thermal Image
      +
Environmental Sensor Data
      +
Time-Series Growth Change
      +
Horticulture Expert Review
      ↓
Crop-Specific Dataset
      ↓
Stress / Growth Diagnostic Model
```

The longer-term objective is a **multi-year greenhouse dataset and diagnostic model** that can support approximately three years of continued collection and refinement.

### Research Axis 3 — Greenhouse Hardware & Integrated Control

The project also includes development of the physical sensing and control layer needed to move from analysis to field operation.

Target hardware / interfaces include:

- RGB / thermal cameras
- temperature / humidity sensors
- soil-moisture sensors
- illuminance sensors
- EC / pH sensors
- Arduino / ESP32-class sensor nodes
- Raspberry Pi-class edge gateway
- communication gateway
- integrated control panel
- relay / actuator interfaces

Initial data-flow concepts include **MQTT / local storage / resend handling** so that greenhouse sensing remains usable even when network conditions are unstable.

The target control devices are:

- irrigation pump / valve
- ventilation
- shading
- spraying / treatment modules

### First PoC — Irrigation Closed Loop

The practical first closed-loop PoC is planned around **irrigation**, because it provides a clear measurable relationship between sensing, decision, actuation, and re-measurement.

```text
Temperature / Humidity
Soil Moisture
Illuminance
RGB Observation
        ↓
Gateway / Data Collection
        ↓
Rule or AI-Assisted Decision
        ↓
Pump / Valve Control
        ↓
Re-measurement
        ↓
Before / After Comparison
```

Once the sensing-to-action loop is stable, the same architecture can be expanded toward heat-stress response, ventilation, shading, spraying, and more autonomous greenhouse operation.

### 2026-10-01 Greenhouse Meeting — Validation Direction

The greenhouse meeting focused on reducing project risk by validating the system in stages instead of attempting the full autonomous system at once.

The practical sequence discussed was:

1. begin with **fixed RGB + environmental sensors**
2. establish repeatable crop / zone IDs and collection procedures
3. compare thermal imagery through fixed or manual acquisition
4. evaluate whether thermal-drone automation adds sufficient value
5. define crop, greenhouse zone, observation interval, equipment ownership, and operating procedures
6. expand toward automatic control only after sensing / diagnosis reliability is demonstrated

Additional field issues under review include:

- greenhouse indoor flight characteristics
- drone operating responsibility
- insurance / safety constraints
- positioning and navigation limitations in greenhouse environments
- SLAM or alternative indoor-localization feasibility
- whether a fixed-camera system is more practical than routine indoor drone operation

### Interdisciplinary Roles

| Area | Responsibility |
| --- | --- |
| **Horticulture / Forestry** | primary crop selection · growth criteria · stress definitions · expert validation |
| **Software / AI** | dataset pipeline · Vision AI · sensor fusion · dashboard · system integration |
| **Electrical / Electronics** | sensors · power · MCU / IoT · gateway · control-panel interfaces |
| **UAV / Robotics** | thermal / RGB remote sensing · flight workflow · automation feasibility |
| **Architecture / Landscape / Greenhouse** | spatial constraints · equipment placement · greenhouse operation context |
| **IT / Project Management** | schedule · records · requirements · milestones · interdisciplinary coordination |

### Development Roadmap

```text
Phase 1
Fixed RGB + Environment Sensors
        ↓
Phase 2
Dataset / Individual or Zone Tracking
        ↓
Phase 3
Thermal Comparison + Stress Detection
        ↓
Phase 4
AI-Assisted Diagnosis / Dashboard
        ↓
Phase 5
Irrigation Closed-Loop Control
        ↓
Phase 6
Ventilation / Shading / Treatment Integration
        ↓
Phase 7
AI Farmer / Autonomous Greenhouse PoC
```

### Current Validation Principle

The project intentionally separates:

- collected data
- AI inference
- horticulture-expert interpretation
- actuator command
- field-verified effect

This is intended to avoid presenting a predicted crop condition as a confirmed agronomic diagnosis before expert and field validation.

**Status:** Ongoing Research / Greenhouse PoC Planning

</details>

---

<details>
<summary><strong>🏥 Healthcare HIS</strong></summary>

**Type:** Healthcare Information System / Interdisciplinary Project  
**Project:** Integrated HIS / Nursing Workflow Platform  
**Role:** Project Planning · Information Architecture · Interdisciplinary Requirements Coordination

### Problem / Objective

The project explores how fragmented healthcare / nursing information and operational workflows can be represented in a unified information-system structure.

### Development / Research

- healthcare information architecture
- nursing-workflow mapping
- user-role / task-flow definition
- multidisciplinary requirement gathering
- operational data-flow concepts
- user-centered system design
- prototype / workflow planning

The emphasis is on understanding real healthcare workflow before defining software features.

**Status:** Planning / Research

</details>

---

<details>
<summary><strong>🏗️ Underground Connection Route GIS Research</strong></summary>

**Type:** GIS / Smart Construction / Spatial Analysis Research  
**Project:** Pai Chai–Mokwon Underground Connection Route Alternatives  
**Role:** Research Planning · GIS Analysis · Route Comparison

### Research

- NASA SRTM elevation data
- OpenStreetMap building / road data
- EPSG:5186 spatial integration
- route generation with different planning priorities
- conceptual longitudinal-profile comparison
- building-footprint intersection analysis
- 30 m spatial screening-buffer comparison
- quantitative trade-off analysis across Route A / B / C

The work is a preliminary GIS-based route comparison and does **not** claim constructability, structural safety, or settlement verification.

**Status:** 2026 Smart ICT Convergence Academic Conference Research

---

</details>

---

<details>
<summary><strong>👶 NEXUS NEST</strong></summary>

**Type:** Early Childhood Education × Software × Spatial Safety  
**Project:** NEXUS NEST  
**Role:** Project Direction · Interdisciplinary Coordination

### Development / Validation

- classroom photo / floor-plan analysis
- circulation-path review
- evacuation-route obstruction detection
- teacher blind-spot review
- layout comparison
- kindergarten field validation
- teacher interviews

**Status:** 2026 Smart ICT Makerthon Project

---

</details>

---

# PAICHAI NEXUS

---

<details>
<summary><strong>Founder & Lab Lead · Organization, Responsibilities & Current Projects</strong></summary>

## Founder & Lab Lead

**Type:** Student-led Interdisciplinary Project Lab  
**Organization:** PAICHAI NEXUS  
**Role:** Founder & Lab Lead

### Responsibilities

- discovering project and research opportunities
- forming multidisciplinary teams
- defining project scope and expected outcomes
- coordinating technical and domain-expert collaboration
- managing schedules, responsibilities, risks, and checkpoints
- connecting development with field / user validation
- preparing prototypes, competitions, research, and presentations
- coordinating collaboration with professors, companies, and university organizations

### Current Project Areas

- 🌱 Smart Seedling AI
- 🏫 Paejae Pick 2.0
- 🧬 BioDockLab
- 🏥 Healthcare HIS
- 🏗️ Tunnel Stability Research
- 🍽️ Zero-Waste FoodTech
- 🤖 ROS2 / autonomous mobility
- 👶 NEXUS NEST
- 🧠 interdisciplinary AI / software projects

> **Interdisciplinary collaboration creates value when each major contributes real domain expertise.**

---

</details>

---

# Technical Stack

### Core Systems

`C` · `C++` · `Python` · `Linux`  
`ROS2` · `PX4` · `MAVLink` · `MAVSDK`

### Embedded / Interfaces

`UART` · `CAN` · `RS485` · `Modbus`  
`GNSS / RTK` · `NMEA` · `NTRIP` · `RTCM`  
`i.MX6` · `Zynq`

### Integration / Backend

`FastAPI` · `REST API` · `WebSocket`  
`Node.js` · `SQLite` · `PostgreSQL`

### AI / Perception / Data

`OpenCV` · `YOLO` · `Telemetry Analysis`

### Validation / DevOps

`Git` · `GitHub` · `Docker` · `pytest` · `GitHub Actions`

### Electronics / Production

`PCB` · `BOM` · `Gerber` · `SMT`

> Frontend and web technologies are used primarily for GCS, control interfaces, operational dashboards, visualization, and system integration rather than as my primary engineering identity.

---

---

# Engineering Labs

---

<details>
<summary><strong>Repository Index</strong></summary>

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

</details>

---

# Selected Outcomes

- 🏆 **Top Prize / 1st Place** — 2026 Future Government Innovation Idea Contest · BioDockLab
- 🏆 **Encouragement Award** — 2026 Intelligent Innovation Idea Contest · Paejae Pick
- 🛩️ **1st Preliminary Passed** — 24th Korea Robot Aircraft Competition · SkyEdge VTOL
- 🎓 **Selected Project** — 2026 NASEOM Competency Maker · Paejae Pick 2.0
- 🔧 **2026 Smart ICT Makerthon** — NEXUS NEST · Early Childhood Education × Spatial Safety
- 📚 **2026 Smart ICT Convergence Academic Conference** — Pai Chai–Mokwon Tunnel Route GIS Research
- 🤝 **2026 Regional Community Problem-Solving Innovative Social Venture Hackathon** — Participation Confirmed
- 🤝 **NEXUS × College of Business Administration** — Poster · Promotional Video · QR Voting · Event-System Support
- 🌲 **Industry R&D** — Disaster Response · UAV/GCS · GNSS/RTK · Field Communication · Integrated Control

---

---

# Engineering Principles

---

<details>
<summary><strong>Engineering Process & Principles</strong></summary>

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

---

</details>

---

# Long-Term Direction

---

<details>
<summary><strong>Technical Growth Path</strong></summary>

```text
Electronics / Embedded
        ↓
Systems & Interfaces
        ↓
UAV / Robotics / Communication
        ↓
Mission Autonomy
        ↓
Physical AI
        ↓
Multi-Unmanned Systems
        ↓
Technical Project Leadership
        ↓
Program / System Leadership
```

**autonomous aerospace · UAV systems · embedded systems · disaster-response systems · Physical AI · multi-unmanned systems · technical program leadership**

---

</details>

---

## GitHub

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=gxmzung&show_icons=true&include_all_commits=true&hide_border=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=gxmzung&layout=compact&hide_border=true)

</div>

> Activity metrics are secondary to repository quality, reproducible engineering work, reviews, and collaboration history.
---

# Contact

- **GitHub:** https://github.com/gxmzung
- **Email:** leeyj4748@naver.com
