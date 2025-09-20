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

### Icarus Verilog (Iverilog)

Iverilog is a Verilog compiler that generates an intermediate format for simulation.

```bash
# Update package list and install Icarus Verilog
$ sudo apt-get update
$ sudo apt-get install iverilog
```

### GTKWave

GTKWave is a waveform viewer used to display simulation results.

```bash
# Update package list and install GTKWave
$ sudo apt-get update
$ sudo apt install gtkwave
```
