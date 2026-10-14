🚦 Traffic Light Controller with Pedestrian Crossing

An FSM-based Traffic Light Controller designed using Verilog HDL and simulated using Xilinx Vivado.

📌 Project Overview

This project implements a Finite State Machine (FSM)-based traffic light controller that manages highway and side-road traffic while supporting pedestrian crossing functionality.

The controller uses clock signals, timer logic, and a pedestrian request input to control traffic signal transitions.

🎯 Objectives

- Design an FSM-based traffic light controller.
- Control highway and side-road traffic signals.
- Implement pedestrian crossing functionality.
- Verify the design using simulation.
- Analyze the RTL schematic and power analysis results using Vivado.

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
2. After the configured timer interval, the highway signal changes to yellow.
3. The controller checks the pedestrian request before selecting the next state.
4. If a pedestrian request is received, the pedestrian crossing state is activated.
5. Otherwise, the controller transitions to the side-road green state.
6. The controller continues switching between traffic states according to the FSM logic.

🔬 Simulation Results

1. RTL Schematic

Shows the RTL design and internal logic connections generated using Xilinx Vivado.

"RTL Schematic" (outputs/rtl-schematic.png)

2. Simulation Waveform

Displays the clock, reset, pedestrian request, highway signals, side-road signals, and pedestrian walk output over time.

"Simulation Waveform" (outputs/simulation-waveform.png)

3. Power Analysis

Shows the power analysis results reported by Vivado for the implemented design.

"Power Analysis" (outputs/power-analysis.png)

4. Console Output

Displays the simulation log and traffic signal values during execution.

"Console Output" (outputs/simulation-console.png)

📁 Project Structure

Traffic-Light-Controller-with-Pedestrian-Crossing/
│
├── README.md
├── traffic_light_controller.v
├── tb_traffic_light_controller.v
│
└── outputs/
    ├── rtl-schematic.png
    ├── simulation-waveform.png
    ├── power-analysis.png
    └── simulation-console.png

📚 Learning Outcomes

Through this project, I gained practical understanding of:

- Verilog HDL programming
- Finite State Machine design
- Sequential logic and timer-based control
- Traffic signal control logic
- Testbench development and simulation
- RTL schematic analysis
- Power analysis using Xilinx Vivado

✅ Conclusion

The Traffic Light Controller with Pedestrian Crossing demonstrates the practical application of FSM concepts in digital system design. The design was simulated using Xilinx Vivado to examine traffic signal transitions and pedestrian crossing behavior.

👩‍💻 Author

Akshaya Reddy
B.Tech — Electronics and Communication Engineering (ECE)
