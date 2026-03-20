# FSAE Rear Hub — Velocita Racing

**Velocita Racing | Formula Student | Ramaiah Institute of Technology**
**Role: Suspension Lead | Competition: Formula Bharat 2025 — P2 Overall, P2 Engineering Design**

---

## Overview

This repository documents the design, analysis, and validation of the rear wheel hub developed for the Velocita Racing FSAE vehicle. The hub is a safety-critical rotating component that interfaces the drivetrain (half-shaft / CV joint), wheel bearing, brake rotor, and wheel assembly. It must reliably transmit traction, braking, and cornering loads under all operating conditions within a strict weight budget.

---

## Repository Structure

```
fsae-rear-hub/
│
├── README.md                        ← You are here
│
├── docs/
│   └── Rear_Hub_Design_Report.md   ← Full engineering design report
│
├── specs/
│   └── hub_specifications.md       ← Material, dimensional & interface specs
│
├── fea/
│   └── fea_summary.md              ← FEA load cases, results & screenshots guide
│
└── drawings/
    └── README.md                   ← Notes on CAD drawings (SolidWorks)
```

---

## Key Specifications at a Glance

| Parameter              | Value                        |
|------------------------|------------------------------|
| Material               | EN24 Steel (817M40)          |
| Yield Strength         | 680 MPa (normalised)         |
| UTS                    | 850 MPa (normalised)         |
| Manufacturing Process  | CNC Machining                |
| Target Factor of Safety| ≥ 1.5                        |
| Car Mass (with driver) | ~275 kg (design midpoint)    |
| Peak Lateral Load (ay) | 1.5g                         |
| Peak Longitudinal (ax) | 1.5g                         |
| Peak Bump Load (az)    | 3.0g                         |
| Bearing Interface      | Press-fit / angular contact  |
| Drive Interface        | Splined (CV joint side)      |

---

## Design Objectives

- Transmit all wheel loads to the upright and suspension geometry without yielding or fatigue failure
- Maintain precise bearing preload and alignment throughout the operating envelope
- Minimise rotating unsprung mass while meeting FoS targets
- Ensure full compliance with Formula Bharat 2025 technical regulations
- Be manufacturable in-house using CNC machining on EN24 bar stock

---

## Load Cases Considered

| Load Case                  | Description                                              |
|----------------------------|----------------------------------------------------------|
| Pure Braking               | 1.5g longitudinal deceleration, rear bias applied        |
| Pure Cornering             | 1.5g lateral acceleration, outer rear worst case        |
| Combined Braking+Cornering | Simultaneous lateral + longitudinal loading (worst case) |
| Bump / Vertical            | 3.0g vertical load simulating kerb strike or rough track |

---

## Tools Used

| Tool                   | Purpose                                      |
|------------------------|----------------------------------------------|
| SolidWorks             | 3D modelling, assembly, and drawing creation |
| Ansys Workbench        | Static structural FEA                        |
| Ansys Mechanical APDL  | Mesh refinement and result extraction        |
| Optimum Kinematics     | Suspension geometry and load transfer calc   |
| MSC Adams              | Multi-body dynamics validation               |

---

## Results Summary

| Load Case                  | Max von Mises Stress | FoS vs Yield (680 MPa) |
|----------------------------|----------------------|------------------------|
| Pure Braking               | ~210 MPa             | ~3.2                   |
| Pure Cornering             | ~260 MPa             | ~2.6                   |
| Combined Braking+Cornering | ~340 MPa             | ~2.0                   |
| Bump / Vertical (3g)       | ~420 MPa             | ~1.6                   |

> All load cases satisfy the minimum FoS of 1.5 against yield. Bump + combined loading governs the design.

---

## Competition Result

**Formula Bharat 2025 — P2 Overall | P2 Engineering Design**

The rear hub design contributed to a suspension system that passed all dynamic events and scrutineering without failure or geometry deviation.

---

## Author

**Drush Subbaiah** — Suspension Lead, Velocita Racing
[LinkedIn](https://linkedin.com/in/DrushSubbaiah) | subbaiahdrush@gmail.com
Ramaiah Institute of Technology, Bengaluru
B.E. Mechanical Engineering | CGPA: 9.13
