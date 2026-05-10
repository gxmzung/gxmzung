# gxmzung

### Embedded Systems · Telemetry · ROS2/PX4 · Smart Campus

I build software around telemetry, field operations, autonomous systems, and campus-scale service infrastructure.

My projects focus on system flow, implementation evidence, realistic constraints, and operation-oriented architecture rather than isolated UI demos.

---

## How I Got Into Programming

I did not start programming only from web or app development.

My interest in software grew from hardware-adjacent work: PCB production flow, BOM handling, datasheet reading, OrCAD-based schematic review, component organization, and debugging around real production processes.

Through that experience, I realized that understanding hardware alone was not enough.

To understand how a real system works, I needed to understand the software layers around it:

- backend logic
- device communication
- telemetry
- monitoring
- automation
- operational interfaces

I first approached software through Java, Spring Boot, Kotlin, and application/backend development.

Over time, my direction moved deeper toward C/C++, embedded-style telemetry, diagnostics, ROS2/PX4 simulation, and ground-control-style systems.

That is why my current projects focus on the boundary between hardware-adjacent data, backend systems, field operations, autonomous systems, and user-facing dashboards.

---

## Tech Stack

### Core

![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)

### Robotics / Systems

![ROS2](https://img.shields.io/badge/ROS2-22314E?style=flat-square&logo=ros&logoColor=white)
![PX4](https://img.shields.io/badge/PX4-005CAF?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

### App / Dashboard

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)

---

## Portfolio Map

### Ground Control / Embedded / Diagnostics

| Repository | Focus |
|---|---|
| [`sat-gcs-defense-space-plus10`](https://github.com/gxmzung/sat-gcs-defense-space-plus10) | Satellite ground-control style telemetry pipeline with C++ packet handling, Java mission server, Python tools, and React dashboard |
| [`fieldops-embedded-diagnostic-suite`](https://github.com/gxmzung/fieldops-embedded-diagnostic-suite) | Embedded field diagnostics toolkit with serial parsing, GNSS tracking, telemetry monitoring, C scheduler logic, log analysis, and dashboard prototype |

### Drone / Autonomous Systems

| Repository | Focus |
|---|---|
| [`twinflight-mission-v2`](https://github.com/gxmzung/twinflight-mission-v2) | ROS2 / PX4 mission simulation with YAML mission config, offboard control flow, and PX4 SITL workflow |
| [`wildtrack-assist`](https://github.com/gxmzung/wildtrack-assist) | Search operation support system with backend, dashboard, drone simulator, report ranking, and AI-assisted validation |

### Smart Campus / Campus Operations

| Repository | Focus |
|---|---|
| [`CityBrain`](https://github.com/gxmzung/CityBrain) | Smart campus cafeteria MVP with FastAPI backend, Android app, admin dashboard, student UI, operation logs, and Jarvis assistant prototype |
| [`paejae-campus-os-v1`](https://github.com/gxmzung/paejae-campus-os-v1) | Smart campus platform scaffold for building metadata, room monitoring, admin dashboard, student services, IoT integration, and digital twin expansion |

---

## Supporting Repositories

| Repository | Role |
|---|---|
| [`skyedge_vtol`](https://github.com/gxmzung/skyedge_vtol) | VTOL mission stack prototype with ROS2-style mission manager, PX4 bridge, safety manager, guidance logic, and vision nodes |
| [`ros2-px4-yaml-param-debug`](https://github.com/gxmzung/ros2-px4-yaml-param-debug) | Small ROS2/PX4 debugging notes focused on YAML parameter validation and mission configuration checks |
| [`Dorm_Mail_Pcu_Style`](https://github.com/gxmzung/Dorm_Mail_Pcu_Style) | Dormitory mail and lost-item management prototype for campus operations |
| [`LingoLink`](https://github.com/gxmzung/LingoLink) | Korean-Spanish voice translation prototype with mobile, backend, and optional firmware-oriented architecture |
| [`Paejae_Apptech`](https://github.com/gxmzung/Paejae_Apptech) | Early Paejae campus app experiment with Flutter and backend prototypes |

---

## Study Repositories

| Repository | Purpose |
|---|---|
| [`Cs_Resources`](https://github.com/gxmzung/Cs_Resources) | Computer science study archive covering C, C++, Java, Python, Linux, data structures, networking, embedded basics, and interview preparation |
| [`University_Archive`](https://github.com/gxmzung/University_Archive) | University learning archive for coursework, project notes, academic records, and long-term study process tracking |

---

## Engineering Style

I try to build projects with:

- clear system boundaries
- realistic constraints
- runnable or inspectable structure
- documentation that explains why the system exists
- implementation evidence beyond screenshots
- honest limitations and future work
- hardware-adjacent or operations-oriented thinking

---

## Current Direction

My current portfolio direction is:

```text
Embedded / telemetry / diagnostics
+ ROS2 / PX4 / autonomous systems
+ smart campus operation platforms
+ backend and field-facing dashboards
```

My goal is to build software that connects hardware-adjacent systems, backend logic, operational data, simulation, and field-facing interfaces.