# DC/DC Buck Converter Design & Simulation in Altium Designer

## Overview

This project presents a complete DC/DC buck converter design implemented in Altium Designer, including schematic capture, PCB layout, and circuit simulation. The converter is designed for efficient voltage regulation with proper component selection and thermal management considerations. The design process includes multi-sheet schematics, PCB layout with proper layer stackup, and transient analysis to validate circuit performance under various operating conditions.

## System Architecture

The design consists of:

* **Multi-sheet schematic** organization for modular design approach
* **Power stage** including switching MOSFET (Q1), diode (D1), and inductor (L?)
* **Control circuitry** with PWM controller (U1) and feedback network
* **Filtering components** (C1, R1, R2) for output stabilization
* **Four-layer PCB** with proper power and ground planes
* **Transient simulation** to analyze voltage regulation and stability

## Design Specifications

* **Design Software:** Altium Designer 25.4.2
* **PCB Layers:** 4 layers (Top, Bottom, 2 Internal)
* **Grid Settings:** 5mil hotspot snap for precise component placement
* **Mechanical Layers:** Multiple layers for fabrication notes and board outline
* **Component Designators:** D1, U1, C1, R1, Q1, R2, L? (Inductor)

## Schematic Design

The schematic is organized across multiple sheets for better readability and modularity:

* **Sheet 1:** Main power stage and controller
* **Sheet 3-6:** Supporting circuitry and filtering networks
* **Hierarchical design** for complex circuit management
* **Proper annotation** and design rule checking

## PCB Layout Features

* **Component Placement:** Optimized for thermal management and signal integrity
* **Routing Strategy:** Separate power and signal paths
* **Layer Stackup:**
  - Top Layer: Components and signal routing
  - Internal Layer 1: Ground plane
  - Internal Layer 2: Power plane
  - Bottom Layer: Additional routing and components
* **Mechanical Layers:** Used for board outline, mounting holes, and fabrication notes

## Simulation Results

Transient analysis was performed to validate the converter's performance:

* **Analysis Type:** Transient Analysis
* **Monitored Nodes:** NetC7_2, NetC7_3, Net47ou_2, Net47_2.NetD7_2
* **Time Range:** 34.543ms to 34.555ms
* **Voltage Range:** -10V to 70V
* **Key Observations:** Stable voltage regulation, proper switching behavior, and acceptable ripple characteristics

## Key Design Considerations

1. **Thermal Management:** Adequate copper pours and component spacing
2. **Signal Integrity:** Proper ground plane and power plane implementation
3. **EMI Reduction:** Careful routing of switching nodes and filtering
4. **Manufacturability:** Standard component packages and clearances
5. **Testability:** Access points for critical signals

## Design Validation

The design was validated through:

* **Design Rule Check (DRC):** Ensuring manufacturing constraints are met
* **Electrical Rule Check (ERC):** Verifying circuit connectivity and proper pin connections
* **Simulation:** Transient analysis confirming circuit operation
* **3D Visualization:** Mechanical fit and component placement verification

## Project Structure
