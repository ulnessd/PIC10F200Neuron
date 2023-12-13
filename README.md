Simulated Neuron Project
Overview

This project is a microcontroller-based simulation of a neuron, specifically designed for the PIC10F200 microcontroller. It aims to mimic the basic electrical properties of a neuron, including the dendritic input, soma processing, and axon output, by using GPIO pins. This simulation can be a valuable tool for educational purposes or as a building block in more complex neural network simulations.
Features

    Dendritic Input Simulation: Uses GP2 as the input pin, emulating the dendrite of a neuron.
    Soma Output: Simulates the neuron's soma by generating a burst refractory period output on GP1.
    Axon Output: Reproduces a sequence of 12 action potentials on GP0, simulating the axon's behavior.
    Configurable Delays: Incorporates delay routines to mimic the timing of action potentials and refractory periods.

Getting Started
Prerequisites

    MPLAB X IDE
    PIC10F200 microcontroller
    A suitable programmer/debugger (e.g., PICkit)

Installation

    Clone the repository:

    bash

    git clone https://github.com/yourusername/simulated-neuron-project.git

    Open the project in MPLAB X IDE.
    Connect your PIC10F200 to the programmer/debugger.
    Compile and upload the program to the microcontroller.

Configuration

The GPIO pins can be reconfigured by modifying the following lines in the assembly code:

assembly

movlw 0b00001100 ; Configure GPIO pins
tris 6           ; Apply configuration

Usage

Once the program is uploaded to the PIC10F200, it will start simulating a neuron's behavior automatically:

    Input: Apply a high signal to GP2 to start the simulation.
    Soma Output: Observe the burst refractory period on GP1.
    Axon Output: Send the 12 action potential bursts on GP0.

