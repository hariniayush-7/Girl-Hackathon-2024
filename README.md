# Girl-Hackathon-2024


# Network on Chip (NOC) Optimization for System on Chip (SoC)

## Introduction

Brief overview of the project and its goals.

## Setup

1. **Requirements**: List the software and hardware prerequisites for running the code. Include specific versions if necessary.
2. **Installation**: Provide step-by-step instructions for setting up the environment. This may include installing dependencies, downloading datasets, or compiling any required libraries.

## Simulator Setup

1. **Configuration**: Explain how to configure the simulator for running simulations. This may involve setting buffer sizes, arbiter weights, and other parameters.
2. **Data Generation**: Outline the process for generating simulation data using the provided APIs or scripts.

## Running the Code

1. **Simulation Execution**: Provide instructions for running simulations using the prepared data and configured simulator.
2. **Performance Measurement**: Explain how to use the provided pseudocode to measure latency and bandwidth from the simulation output.

## Simulation Environment 

1. **SystemVerilog Simulator**: You'll need access to a SystemVerilog simulator such as ModelSim, VCS, QuestaSim, or Synopsys VCS. These simulators allow you to compile and simulate SystemVerilog code.

2. **Testbench Infrastructure**: You'll need to create a testbench infrastructure to provide monitor output and simulate the behavior of the system under test (SoT). This may involve generating monitor output, initializing signals, and driving inputs to the SoT.

3. **Monitor Output Generation**: You'll need to implement the `read_monitor_output()` function to read monitor output from the testbench infrastructure. This function should return a `MonitorOutput` structure representing the type, agent, and latency of each operation.

4. **Simulation Time Measurement**: You'll need to implement the `get_simulation_time()` function to obtain the simulation time. This function should return the current simulation time in cycles.

5. **Compilation and Simulation**: Once you have set up the environment and implemented the necessary functions, you can compile the SystemVerilog code using the simulator's compiler and run the simulation. The simulation will execute the `MeasureLatencyAndBandwidth()` task, which measures the average latency and bandwidth based on the provided monitor output.

 ## How to run the code
1. Set up your working directory and environment to include the SystemVerilog code file containing the `LatencyAndBandwidthMeasurement` module.

2. Implement the `read_monitor_output()` function to read monitor output from your testbench infrastructure. Ensure that it returns a `MonitorOutput` structure representing the monitor output.

3. Implement the `get_simulation_time()` function to obtain the current simulation time in cycles.

4. Compile the SystemVerilog code using your chosen simulator's compiler. This typically involves invoking the simulator's command-line interface (CLI) and providing the necessary compile flags and options.

5. Once the compilation is successful, run the simulation using the simulator's run command. This will execute the `MeasureLatencyAndBandwidth()` task, which measures the average latency and bandwidth based on the provided monitor output.

6. Monitor the simulation progress and observe the results displayed by the `$display` statements in the code. These statements will show the average CPU read latency, average IO read latency, and bandwidth calculated during the simulation.

7. Analyze the results to assess the performance of the system under test in terms of latency and bandwidth.

## Reinforcement Learning

1. **Setup**: Describe how to set up the RL environment and algorithms for optimizing NOC parameters.
2. **Training**: Provide guidelines for training the RL model using the simulation data.
3. **Evaluation**: Explain how to evaluate the trained model's performance and iterate on the NOC design.

## Usage

1. **Interpreting Results**: Guide users on how to interpret simulation results and RL model outputs.
2. **Troubleshooting**: Include troubleshooting tips for common issues users may encounter.
3. **Example Scripts**: Provide sample scripts or configurations for running simulations and training RL models.



