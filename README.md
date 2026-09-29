## 🔐 Website Login Credentials

Interested in exploring our website? You can use the demo credentials below:

**Username:** hackfusion  
**Password:** yoi time

👉 Open the live website: [Fleet Recovery](https://varshinigadwala50-max.github.io/fleetrecovery/)

> These credentials are provided only for demonstration purposes.
# FleetGuard — Robot Fleet Recovery

> A frontend prototype for monitoring, analyzing, and recovering autonomous robot fleets under cascading failures.

## 📌 Overview

**FleetGuard** is a web-based robot fleet operations interface designed around the problem of **robot fleet recovery under cascading failures**.

The project provides a simulated operator console where users can monitor robot health, identify at-risk units, visualize fleet dependencies, analyze failure propagation, and explore recovery strategies.

The current version is implemented as a **frontend prototype and interactive simulation**. It focuses on demonstrating the user interface, system workflow, visualization, and recovery concepts rather than providing a production backend or real robot integration.

---

## 🎯 Problem Statement

Modern autonomous robot fleets may depend on multiple interconnected units working together to complete missions.

When one robot fails, its failure can affect:

- Task allocation
- Mission completion
- Fleet availability
- Resource utilization
- Dependent robots
- Overall operational continuity

This can result in a **cascading failure**, where the impact of one failed unit spreads through the fleet.

FleetGuard explores how an operator could detect these situations and initiate recovery actions before the failure propagates further.

---

## 💡 Proposed Solution

FleetGuard provides a centralized operations console that allows an operator to:

- Monitor the overall fleet
- Inspect individual robot health
- Identify robots at risk
- Analyze dependencies between units
- Visualize failure propagation
- Review recovery strategies
- Reassign work to healthy robots
- Simulate recovery scenarios

The interface is designed around the concept of **visibility → analysis → recovery**.

---

## 🚀 Key Features

### 1. Command Center

The Command Center provides an overview of the current fleet state.

It displays:

- Online robots
- At-risk robots
- Reassigned jobs
- Fleet survival indicators
- Mission completion
- Robot-level status cards

Operators can select individual robots for further analysis.

---

### 2. Fleet Health Monitoring

The Fleet Health section provides a telemetry-style view of the fleet.

It includes information such as:

- Robot status
- Health
- Battery
- Current task
- Operating zone
- Task speed

This provides a centralized view of fleet health and operational conditions.

---

### 3. 3D Digital Twin

FleetGuard includes a simulated **3D Digital Twin** interface representing an industrial robot cell.

The interface allows users to:

- Inspect robot units
- View simulated robot positions
- Interact with the scene
- Inspect robot metrics
- View dependencies
- Observe potential cascade impacts

The current implementation is a simulated visualization and is not connected to physical robots or live industrial telemetry.

---

### 4. Failure Propagation Analysis

The Failure Propagation section focuses on understanding how the failure of one robot can affect dependent units.

The interface visualizes:

- Failure impact
- Robot dependencies
- Risk information
- Propagation paths
- Recovery considerations

This feature demonstrates the core concept behind cascading failures in a robot fleet.

---

### 5. Recovery Plans

FleetGuard provides multiple recovery strategies that an operator can review before activation.

Recovery decisions can consider different priorities, including:

- Fastest recovery
- Lowest disruption
- Protecting critical missions
- Stopping the cascade first

This demonstrates how different recovery objectives can lead to different operational decisions.

---

### 6. Simulation Lab

The Simulation Lab provides an interactive environment for exploring fleet behavior and recovery scenarios.

It is intended to demonstrate how changes in fleet conditions can influence:

- Efficiency
- Failure impact
- Recovery behavior
- Fleet performance

---

### 7. Manual Task Reassignment

When a robot becomes unavailable, FleetGuard allows the operator to manually assign affected work to another available robot.

This represents one possible recovery mechanism for maintaining mission continuity.

---

### 8. Interactive Operator Console

The project includes an operator-oriented interface with:

- Operator access screen
- Dashboard navigation
- Robot inspection
- Alerts
- Recovery actions
- Interactive controls
- Sign-out functionality

---

## 🛠️ Technology Stack

### Frontend

- **HTML5**
- **CSS3**
- **JavaScript**
- **Canvas API**
- Responsive CSS layouts
- CSS animations and transitions

The interface uses custom HTML/CSS styling and JavaScript-driven interactions. The source also uses web fonts including **Inter** and **JetBrains Mono**. :contentReference[oaicite:1]{index=1}

---

## 🏗️ Project Architecture

```text
FleetGuard
│
├── Landing / Overview
│
├── Operator Access
│
└── Operations Console
    │
    ├── Command Center
    │
    ├── Fleet Health
    │
    ├── 3D Digital Twin
    │
    ├── Recovery Plans
    │
    ├── Failure Propagation
    │
    └── Simulation Lab
