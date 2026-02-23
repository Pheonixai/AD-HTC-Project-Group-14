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
---

Thermodynamic Process Stages
StageProcessDescriptionABiogas GenerationCalculates biomass maturity duration and total biogas flow rate from dry mass inputs and methane yield metricsBIsentropic CompressionModels ambient air pressurization and the temperature rise preceding combustionCFuel-Enhanced CombustionEvaluates thermal boost from injecting biogas and HTC volatiles into the combustion chamberDTurbine Expansion & ExhaustMeasures mechanical power from gas expansion and tracks exhaust temperature (T₄) recycled to the HTC boilerNetPower OutputComputes final electrical yield after subtracting parasitic loads (compression, auxiliary systems)

System Outputs
---

⚡ Electricity — Net power output from the gas turbine cycle
🔥 Biogas — Usable biomethane from anaerobic digestion
🪨 Bio-Coal (Hydrochar) — Solid carbon-rich fuel from HTC, suitable for further combustion or soil amendment


Strategic Advantages
---

Thermal Independence — Exhaust heat recycling eliminates external energy inputs for the HTC reactor
Carbon-Neutral Operation — Closed-loop biomass cycle with no net fossil CO₂ emissions
Waste Valorization — Converts low-value organic waste into three high-value outputs
Dispatchable Power — Unlike intermittent solar/wind, output is controllable and on-demand
GHG Mitigation — Prevents methane venting from unmanaged waste decomposition


**Getting Started**
---
Prerequisites

List your runtime requirements here (e.g., Python 3.10+, Node.js, specific libraries).

bash# Example
pip install -r requirements.txt
Installation
bashgit clone https://github.com/your-username/ad-htc-simulator.git
cd ad-htc-simulator
# Add setup steps here
Running the Application
bash# Add your launch command here
python main.py

**Roadmap**
---

 Dynamic biomass composition inputs (multi-feedstock support)
 Economic modeling module (LCOE, ROI analysis)
 Integration with real-world plant sensor data (SCADA/IoT)
 Export simulation results to PDF/CSV
 Multi-scenario batch simulation


**Use Cases**
---

Engineering Design — Size and optimize components for real bioenergy plant projects
Research & Academia — Validate thermodynamic models and explore system configurations
Policy Analysis — Assess techno-economic viability of waste-to-energy deployments


**License**
---
MIT LICENSE