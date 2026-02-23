**AD-HTC Fuel-Enhanced Power Gas Cycle Simulator**
---
A thermodynamic simulation tool for modeling closed-loop waste-to-energy systems integrating Anaerobic Digestion (AD) and Hydrothermal Carbonization (HTC).


**Overview**
----
The AD-HTC application models a synergistic waste-to-energy process that converts low-value organic biomass (e.g., cow dung) into dispatchable electricity, biogas, and bio-coal — while minimizing external energy demands.
The system's key innovation is thermal self-sufficiency: turbine exhaust heat (>400°C) is recycled to sustain the HTC reactor at 180°C, eliminating the need for external heating inputs.
This tool is designed for engineers, researchers, and policymakers who need a robust platform to simulate, analyze, and optimize multi-stage bioenergy recovery systems.

Key Features
---

Modular System Configuration — Independent modules for AD Setup, HTC Boiler Logic, and Power Analysis allow isolated variable adjustment across each subsystem.
Real-Time Thermodynamic Feedback — Instant calculation of pressure, temperature, and enthalpy across all system states for rapid prototyping and operational tuning.
T-H (Enthalpy-Temperature) Graphing — Visual steam cycle monitoring that enforces safe operating bounds within the 180°C HTC reactor, preventing overheating or underperformance.


**System Architecture**
Thermodynamic Process Stages
---
A. Biogas Generation - Calculates biomass maturity duration and total biogas flow rate from dry mass inputs and methane yield metrics
B. Isentropic Compression - Models ambient air pressurization and the temperature rise preceding combustion
C. Fuel-Enhanced Combustion - Evaluates thermal boost from injecting biogas and HTC volatiles into the combustion chamber
D. Turbine Expansion & Exhaust - Measures mechanical power from gas expansion and tracks exhaust temperature (T₄) recycled to the HTC boiler
Net Power Output - Computes final electrical yield after subtracting parasitic loads (compression, auxiliary systems)

System Outputs
---

⚡ Electricity — Net power output from the gas turbine cycle

🔥 Biogas — Usable biomethane from anaerobic digestion

🪨 Bio-Coal (Hydrochar) — Solid carbon-rich fuel from HTC, suitable for further combustion or soil amendment



**Installation**
---
bashgit clone https://github.com/Pheonixai/AD-HTC-PROJECT-GROUP-14-MEG-315.git
cd 315 COURSE PROJECT
 Run the index.html

**License**
---
MIT LICENSE