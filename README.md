🚦 Traffic Light Controller with Pedestrian Crossing

An FSM-based Traffic Light Controller designed using Verilog HDL and simulated using Xilinx Vivado.

📌 Project Overview

This project implements a Finite State Machine (FSM)-based traffic light controller that manages highway and side-road traffic while supporting pedestrian crossing functionality.

🎯 Objectives

- Design an FSM-based traffic light controller.
- Control highway and side-road traffic signals.
- Implement pedestrian crossing functionality.
- Verify the design using simulation.
- Analyze RTL schematic and power analysis results.

🛠️ Technologies Used

- Verilog HDL
- Xilinx Vivado
- Finite State Machine (FSM)
- RTL Design and Simulation
- Verilog Testbench

💻 Design Modules

- "traffic_light_controller.v" — Main Verilog design code.
- "tb_traffic_light_controller.v" — Testbench for simulation and verification.

⚙️ FSM States

State| Description
"HW_GREEN"| Highway green; side road red
"HW_YELLOW"| Highway yellow; side road red
"SR_GREEN"| Side-road green; highway red
"PED_STATE"| Both vehicle signals red; pedestrian walk enabled

🔄 Working Principle

1. The controller starts in the highway green state after reset.
2. The highway signal changes to yellow after the configured timer interval.
3. The controller checks the pedestrian request.
4. If a pedestrian request is received, the pedestrian crossing state is activated.
5. Otherwise, the controller transitions to the side-road green state.
6. The controller continues switching between states according to the FSM logic.

🔬 Simulation Results

1. RTL Schematic

"RTL Schematic" (outputs/rtl-schematic.jpg)

2. Simulation Waveform

"Simulation Waveform" (outputs/simulation-waveform.jpg)

3. Power Analysis

"Power Analysis" (outputs/power-analysis.jpg)

4. Console Output

"Console Output" (outputs/simulation-console.jpg)



📚 Learning Outcomes

- Verilog HDL programming
- Finite State Machine design
- Sequential logic and timer-based control
- Traffic signal control logic
- Testbench development and simulation
- RTL schematic analysis
- Power analysis using Xilinx Vivado

✅ Conclusion

This project demonstrates the application of FSM concepts in digital system design using Verilog HDL. The design was simulated using Xilinx Vivado to examine traffic signal transitions and pedestrian crossing behavior.

👩‍💻 Author

Akshaya Reddy
B.Tech — Electronics and Communication Engineering (ECE)
