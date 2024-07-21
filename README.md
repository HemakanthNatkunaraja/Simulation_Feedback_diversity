
# Simulation_Feedback_Diversity

## Feedback Diversity System

This project demonstrates the implementation of a feedback diversity system for wireless communication using MATLAB and Simulink. The system improves signal reliability by selecting the stronger signal between two SISO fading channels and applying a moving average filter for noise reduction.

## Table of Contents
- [Project Description](#project-description)
- [Model Components](#model-components)
- [Files](#files)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Simulation](#simulation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Description

The feedback diversity system enhances wireless communication by utilizing two SISO fading channels and AWGN channels. The key steps include:
1. Generating a sine wave input signal.
2. Quantizing the signal for 8-PSK modulation.
3. Modulating the signal using an 8-PSK modulator.
4. Passing the signal through SISO fading channels and AWGN channels.
5. Using a feedback diversity selector to choose the stronger signal.
6. Applying a moving average filter to smooth the selected signal.
7. Displaying the final output on a Scope.

## Model Components

### Input Signal
- **Sine Wave**: Generates a continuous sine wave as the input signal.

### Quantizer
- **Quantizer**: Converts the sine wave into discrete levels suitable for 8-PSK modulation.

### Modulator
- **8-PSK Modulator**: Modulates the quantized signal into an 8-PSK signal.

### Channels
- **SISO Fading Channel**: Simulates fading effects on the modulated signal.
- **AWGN Channel**: Adds white Gaussian noise to the faded signal.

### Feedback Diversity Selector Subsystem
- **Comparator and Switch**: Compares the signal strengths and selects the stronger signal.

### Moving Average Subsystem
- **Moving Average Filter**: Smooths the selected signal to reduce noise.

### Output Signal
- **Scope**: Displays the final processed signal.

## Files

- **Simulink Model**: [Feedback_Diversity.slx](./Feedback_Diversity.slx)
- **MATLAB Code**: [FEEdback_div_code.m](./FEEdback_div_code.m)

## Getting Started

### Prerequisites

- MATLAB with Simulink installed.
- Communications System Toolbox for the modulation and channel blocks.

### Installation

1. Clone this repository to your local machine:
    ```sh
    git clone https://github.com/your_username/Simulation_Feedback_Diversity.git
    cd Simulation_Feedback_Diversity
    ```

2. Open the Simulink model file in MATLAB:
    ```matlab
    open('Feedback_Diversity.slx')
    ```

3. Run the MATLAB script:
    ```matlab
    FEEdback_div_code
    ```

## Usage

1. Open the Simulink model and ensure all blocks are correctly connected.
2. Run the Simulink model to start the simulation.
3. Observe the results on the Scope block to analyze the performance of the feedback diversity system.

## Simulation

The simulation involves the following steps:
1. Generating a sine wave as the input signal.
2. Quantizing and modulating the signal using 8-PSK modulation.
3. Passing the signal through SISO fading channels and AWGN channels.
4. Selecting the stronger signal using a feedback diversity selector.
5. Applying a moving average filter to the selected signal.
6. Displaying the final output on the Scope block.

## Results

The output displayed on the Scope block will show the smoothed and noise-reduced signal after applying the feedback diversity technique.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

