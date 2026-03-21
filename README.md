# FSAE Rear Hub Design
Structural design and analysis of a Formula Student rear wheel hub developed for the Velocita Racing car.  
This project focuses on designing a lightweight yet structurally robust hub capable of transmitting drivetrain torque and handling worst-case suspension loads encountered during racing conditions.

---

## Project Overview
The rear hub is the central rotating component of the rear corner assembly.  
It interfaces the CV joint half-shaft, wheel bearing, brake rotor, and wheel, and must transmit traction and braking torque while reacting lateral, longitudinal, and vertical forces into the upright and suspension structure.

### Objectives
- Minimize rotating unsprung mass
- Maintain structural integrity under peak loads
- Ensure safety factor above acceptable limits
- Integrate with upright, CV joint, bearing, and wheel assembly

---

## Load Case Calculations
Worst-case loads were calculated based on vehicle dynamics and maximum expected racing conditions.

### Considered Load Cases
1. **Braking Load**
2. **Cornering Load**
3. **Vertical Bump Load**
4. **Combined Load Case**

The loads were applied to simulate the worst-case stresses experienced by the hub.

---

## Design Process
1. Determine drivetrain and suspension geometry constraints
2. Calculate worst-case loads from vehicle dynamics
3. Create CAD model in SolidWorks
4. Perform Finite Element Analysis in ANSYS
5. Optimize geometry to reduce rotating mass

---

## CAD Model
Below is the CAD model of the rear hub.

![Hub CAD Isometric 1](https://github.com/DrushSubbaiah/FSAE-Wheel-Hub/blob/main/Screenshot%202026-03-21%20093057.png?raw=true)
![Hub CAD Isometric 2](https://github.com/DrushSubbaiah/FSAE-Wheel-Hub/blob/main/Rear%20section.png)
![Hub CAD Section View](https://github.com/DrushSubbaiah/fsae-upright-design/blob/main/rear%20iso.png)
![Hub CAD Section View](https://github.com/DrushSubbaiah/fsae-upright-design/blob/main/rear%20iso2.png?raw=true)

---

## Load Application
For structural validation, the calculated loads were applied at the wheel flange and bearing seat, representing real suspension, drivetrain, and braking connections.

![Load Case Diagram 1](https://github.com/DrushSubbaiah/fsae-upright-design/blob/main/Screenshot%202026-03-14%20150200.png?raw=true)
![Load Case Diagram 2](https://github.com/DrushSubbaiah/fsae-upright-design/blob/main/Screenshot%202026-03-14%20150216.png?raw=true)

---

## Finite Element Analysis
FEA was conducted to evaluate stress distribution and deformation under worst-case loading conditions.

### Factor of Safety Distribution
![FOS Plot](https://github.com/DrushSubbaiah/FSAE-Wheel-Hub/blob/main/rear%20hub%20FOS.png?raw=true)

### Deformation
![Stress](https://github.com/DrushSubbaiah/FSAE-Wheel-Hub/blob/main/rear%20hub%20deform.png?raw=true)

---

## Results
| Parameter | Value |
|-----------|-------|
| Material | EN24 Steel (817M40) |
| Maximum Stress | 420 MPa |
| Safety Factor | 1.6 |
| Weight | ~850 g |

The design satisfies the required structural criteria while maintaining minimal rotating mass.

---

## Tools Used
- CAD: SolidWorks
- Simulation: ANSYS Workbench / APDL
- Calculations: MS Excel

---

## Key Learnings
- Structural design under combined torsional and bending loading
- Drivetrain-suspension interface integration
- FEA-driven design optimization for rotating components
- Load estimation for motorsport hub and bearing systems

---

## Team
Velocita Racing – Formula Student Team  
Role: **Lead Suspension Engineer**

---

## Future Improvements
- Topology optimization for further mass reduction
- Fatigue analysis for endurance load cycles
- Integrated hub-upright assembly analysis

---

## Author
Drush Subbaiah  
Mechanical Engineering Student  
Formula Student Suspension Lead  
Velocita Racing
