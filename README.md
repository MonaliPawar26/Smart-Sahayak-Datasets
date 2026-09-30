
# 🤖 Smart Sahayak — AMR Dataset Repository

> Dataset collection for **Smart Sahayak**, an Edge-AI based distributed fleet coordination system for Autonomous Mobile Robots (AMRs) in smart warehouses.

Smart Sahayak focuses on enabling multiple AMRs to coordinate tasks, communicate locally, avoid conflicts, and continue operating under changing warehouse and network conditions.

This repository contains structured datasets for representing robots, warehouse scenarios, tasks, and system events used during Smart Sahayak development and evaluation.

---

## 🎯 Project Objective

The datasets are designed to support the development and testing of:

- Distributed AMR coordination
- Dynamic task allocation
- Contract-Net based task assignment
- Robot-to-robot communication
- Multi-robot path planning
- Conflict and collision detection
- Dynamic re-planning
- Network-degraded operating scenarios
- Battery and workload-aware decisions
- Warehouse task execution

---

## 📂 Repository Structure

```text
Smart-Sahayak-Datasets/
│
├── events/
│   └── Robot and system event data
│
├── robots/
│   └── AMR state and robot data
│
├── scenarios/
│   └── Warehouse operating scenarios
│
├── tasks/
│   └── Task allocation and execution data
│
├── all_datasets.json
└── README.md
````

---

## 🤖 Robots Dataset

The `robots/` directory contains data representing individual AMRs and their operational states.

The dataset supports information related to:

* Robot ID
* Position
* Battery level
* Current task
* Workload
* Availability
* Robot status
* Current route
* Operating state

This data supports distributed decision-making and fleet coordination.

---

## 📦 Tasks Dataset

The `tasks/` directory contains warehouse task information used for task allocation and execution.

Tasks represent information such as:

* Pickup location
* Destination
* Priority
* Task requirements
* Estimated travel cost
* Task status
* Assignment information

This dataset supports the **Contract-Net based task allocation** mechanism used in Smart Sahayak.

---

## 🏭 Scenarios Dataset

The `scenarios/` directory represents different warehouse operating conditions.

Scenarios include conditions such as:

* Normal warehouse operation
* High-congestion areas
* Blocked aisles
* Dynamic obstacles
* Multiple AMR operations
* Communication degradation
* Robot unavailability

These scenarios help evaluate distributed fleet behaviour under changing conditions.

---

## ⚠️ Events Dataset

The `events/` directory contains robot and system events generated during operations.

Examples include:

* Task announcement
* Task assignment
* Movement intent
* Conflict detection
* Blocked aisle
* Battery warning
* Communication degradation
* Re-planning
* Re-auction
* Task completion

These events help analyse the decision-making and recovery process.

---

## 📊 Combined Dataset

The `all_datasets.json` file provides a consolidated representation of the available datasets.

It can be used for:

* Model development
* Simulation
* Algorithm testing
* Scenario generation
* Performance evaluation
* AMR coordination experiments

---

## 🔄 Smart Sahayak Data Flow

```text
Warehouse Scenario
        ↓
Task Generation
        ↓
Task Announcement
        ↓
Contract-Net Allocation
        ↓
AMR Selection
        ↓
P2P Coordination
        ↓
Path Planning
        ↓
Conflict Detection
        ↓
Move / Wait / Re-plan
        ↓
Task Execution
        ↓
Task Completed / Recovery
```

---

## 🧠 Dataset Applications

### 1. Dynamic Task Allocation

Selecting suitable AMRs using factors such as travel cost, battery, workload, and availability.

### 2. Multi-Robot Coordination

Studying how multiple AMRs coordinate without depending entirely on a centralized controller.

### 3. Path Planning

Testing route planning and reservation-based movement in shared warehouse environments.

### 4. Conflict Resolution

Evaluating robot behaviour when multiple AMRs encounter potential path conflicts.

### 5. Dynamic Recovery

Testing re-planning and task re-auction when an aisle becomes blocked or a robot becomes unavailable.

### 6. Network Resilience

Evaluating fleet behaviour under normal and degraded communication conditions.

---

## 🛠️ Technology Context

The datasets support the Smart Sahayak system architecture using technologies and methods such as:

* **ROS 2** — Robot middleware
* **Python** — Edge intelligence and processing
* **LiDAR / Odometry** — Perception and localization
* **Contract-Net Protocol** — Task allocation
* **A*** — Path planning
* **Reservation Tables** — Space-time coordination
* **P2P Communication** — Distributed coordination
* **MQTT-SN / CoAP / UDP** — Network communication
* **Gazebo** — Robot simulation

---

## 📈 Smart Sahayak Architecture

```text
                 SMART WAREHOUSE
                        │
                        ▼
                TASK ANNOUNCEMENT
                        │
                        ▼
               CONTRACT-NET AUCTION
                        │
                        ▼
              DISTRIBUTED AMR FLEET
                 ┌──────┼──────┐
                 ▼      ▼      ▼
              AMR 01  AMR 02  AMR 03
                 │      │      │
                 └──────┼──────┘
                        ▼
                 P2P COORDINATION
                        │
                        ▼
                 EDGE-AI CONTROL
                        │
                        ▼
              SPACE-TIME PLANNING
                        │
                        ▼
               CONFLICT DETECTION
                        │
                 ┌──────┴──────┐
                 ▼             ▼
               MOVE       WAIT / RE-PLAN
                 │             │
                 └──────┬──────┘
                        ▼
                 SAFE EXECUTION
```

---

## 🔬 Research Focus

The dataset repository supports experimentation in:

* Decentralized Multi-Agent Path Finding
* Multi-Agent Pickup and Delivery
* Contract-Net task allocation
* Edge-based robot coordination
* Collision avoidance
* Dynamic path planning
* Network-resilient robotics
* Smart warehouse automation

---

## 🚀 Future Dataset Expansion

Future versions may include:

* Larger AMR fleets
* More complex warehouse layouts
* Real sensor streams
* LiDAR point-cloud data
* Battery consumption traces
* Communication latency measurements
* Congestion measurements
* Dynamic obstacle scenarios
* Real-world AMR logs
* Simulation-generated benchmark datasets

---

## 📌 Project Information

**Project:** Smart Sahayak

**Title:** Edge-AI Based Distributed Fleet Coordination for Autonomous Mobile Robots (AMRs) in Smart Warehouses

**Problem Statement:** SIH 2026 — PS 26123

**Repository:** Smart-Sahayak-Datasets

---

## 👥 Contributors

Developed as part of the **Smart Sahayak** project for Smart India Hackathon.

---
## 📄 License

This repository is intended for academic, research, simulation, and prototype development purposes.


