# Sequence Detector (Moore FSM) Project

This project implements a **Sequence Detector** using a Moore Finite State Machine (FSM) in Verilog. The system detects a predefined sequence in a serial input stream and asserts an output signal when the sequence is detected. The project includes the Verilog module and a testbench for simulation.

## Project Structure

The project contains the following files:

1. `Sequence_Detector_MOORE_Verilog.v`
   - The main Verilog module implementing the sequence detector using Moore FSM principles.
2. `tb_Sequence_Detector_Moore_FSM_Verilog.v`
   - A testbench for simulating the sequence detector.

## Features

- Implements a Moore FSM to detect a specific sequence in a serial data stream.
- Configurable reset signal to initialize the FSM.
- Includes a testbench for verification of functionality with multiple test cases.

## Prerequisites

To run or simulate this project, you need the following tools installed:

- **Verilog Simulator**: Use one of the following:
  - ModelSim
  - Icarus Verilog 
  - Synopsys VCS
  - Cadence Xcelium
    
## How to Simulate

1. Clone this repository to your local machine:
   ```bash
   git clone <repository_url>
   cd <repository_name>
   ```

2. Compile the Veilog files:
   ```bash
   iverilog -o Sequence_Detector_MOORE Sequence_Detector_MOORE_Verilog.v tb_Sequence_Detector_Moore_FSM_Verilog.v
   ```
4. Run the simulation:
   ```bash
   vvp Sequence_Detector_MOORE
   ```
## Verilog Module

The `Sequence_Detector_MOORE_Verilog` module uses a Moore FSM with five states:
  - `Zero`
  - `One`
  - `OneZero`
  - `OneZeroOne`
  - `OneZeroOneOne`
![image](https://github.com/user-attachments/assets/6570f571-082b-4568-88e9-7c9c7da72d35)
## Output diagram:
![image](https://github.com/user-attachments/assets/8468ebaf-a822-4e5a-a0d5-392545165d7e)
![image](https://github.com/user-attachments/assets/d90e8fef-31a1-415d-997e-f7d84eeef963)

## Testbench

The testbench provides a clock generator, reset signal, and test sequences to validate the functionality of the sequence detector. The simulation includes:
  - Initial reset to set the FSM to the initial state.
  - Various input sequences to test all possible state transitions.

