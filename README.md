# Subh27_RISC-V
# Week 0 Task – Environment Setup

This document describes the initial setup required for participating in the VSD RISC-V Tapeout Program. It includes installation of the necessary operating system, tools, and dependencies.

# System Requirements

Operating System: Ubuntu 20.04 or higher
RAM: Minimum 6 GB
Storage: Minimum 50 GB HDD/SSD
CPU: Minimum 4 vCPUs

# Download Oracle VirtualBox for setting up the environment:
VirtualBox Downloads

# Tool Installation
# 1. Yosys (Logic Synthesis Tool)

Yosys is used for RTL synthesis.

sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt-get install make build-essential clang bison flex \
libreadline-dev gawk tcl-dev libffi-dev git \
graphviz xdot pkg-config python3 libboost-system-dev \
libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc
make
sudo make install

# 2. Icarus Verilog (Simulation Tool)

Icarus Verilog is used for compiling and simulating Verilog code.

sudo apt-get update
sudo apt-get install iverilog

# 3. GTKWave (Waveform Viewer)

GTKWave is used to view simulation waveforms.

sudo apt-get update
sudo apt-get install gtkwave

sudo apt-get update
sudo apt-get install gtkwave
