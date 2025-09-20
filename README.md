# Subh27_RISC-V

# Week 0 Task

This document outlines the setup instructions and system requirements for completing the Week 0 task.

## Prerequisites

### 1\. Oracle VirtualBox

Download and install the Oracle VirtualBox from the official website. This is required to set up the Ubuntu virtual machine.

  * **Link**: [https://www.virtualbox.org/wiki/Downloads](https://www.virtualbox.org/wiki/Downloads)

### 2\. System Requirements

Ensure your system meets the following specifications for the virtual machine.

  * **RAM**: At least 6 GB
  * **HDD**: At least 50 GB of free space
  * **Operating System**: Ubuntu 20.04 or higher
  * **vCPU**: At least 4 virtual CPUs

-----

## Tool Installation

Follow the steps below to install the necessary tools for the project.

### Yosys

Yosys is an open-source framework for Verilog RTL synthesis.

```bash
# Update package list
$ sudo apt-get update

# Clone the Yosys repository
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys

# Install dependencies and build tools
$ sudo apt install make
$ sudo apt-get install build-essential clang bison flex \
libreadline-dev gawk tcl-dev libffi-dev git \
graphviz xdot pkg-config python3 libboost-system-dev \
libboost-python-dev libboost-filesystem-dev zlib1g-dev

# Configure, build, and install Yosys
$ make config-gcc
$ make
$ sudo make install
```
<img width="790" height="547" alt="Screenshot from 2025-09-20 23-28-28" src="https://github.com/user-attachments/assets/8dc6fd63-c7ae-458d-8660-63d7a518aa86" />
<img width="790" height="529" alt="Screenshot from 2025-09-20 23-28-53" src="https://github.com/user-attachments/assets/a8f4dbdb-cfab-46b4-9e3f-2d3e13121b4e" />

### Icarus Verilog (Iverilog)

Iverilog is a Verilog compiler that generates an intermediate format for simulation.

```bash
# Update package list and install Icarus Verilog
$ sudo apt-get update
$ sudo apt-get install iverilog
```
<img width="790" height="529" alt="Screenshot from 2025-09-20 23-29-27" src="https://github.com/user-attachments/assets/2f4db6e1-72b7-4220-a543-aa95e91ea232" />

### GTKWave

GTKWave is a waveform viewer used to display simulation results.

```bash
# Update package list and install GTKWave
$ sudo apt-get update
$ sudo apt install gtkwave
```
<img width="795" height="594" alt="Screenshot from 2025-09-20 23-30-03" src="https://github.com/user-attachments/assets/ae4a4687-7e59-4463-9705-571b459a7b84" />

### Tool Version Check

This section shows the commands to verify the installed versions of essential tools.

```bash

$ git --version
$ make --version
$ g++ --version
$ gcc --version
```
<img width="795" height="594" alt="Screenshot from 2025-09-20 23-30-57" src="https://github.com/user-attachments/assets/e51ca223-cfd7-4e2f-8ec3-d16fa1871509" />
<img width="795" height="594" alt="Screenshot from 2025-09-20 23-38-41" src="https://github.com/user-attachments/assets/100e4d5f-f232-4796-9ad1-506aaf2eb89d" />


