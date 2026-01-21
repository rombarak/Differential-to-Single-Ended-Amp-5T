# Differential to Single Ended Operational Amplifier (5T) Design

## Project Overview
This repository contains the design and analysis of a **5-Transistor (5T) Differential to Single-Ended Operational Amplifier**, implemented in **Cadence Virtuoso**. The project explores the fundamentals of differential pair stages, current mirror biasing, and the trade-offs between gain, bandwidth, and stability in a unity-gain configuration.

## Key Specifications & Performance
* **Open-Loop Gain:** ~51 dB.
* **Phase Margin (PM):** 86.84° (High stability margin).
* **Unity Gain Bandwidth (UGB):** ~7.35 MHz.
* **Output Load:** 0.2 pF.
* **Slew Rate:** Measured and analyzed for both rising and falling edges to evaluate large-signal behavior.
* **Settling Time:** Approximately 135.5 ns.

## Design Highlights
* **Architecture:** 5-Transistor (5T) topology featuring a PMOS differential pair and an NMOS current mirror load.
* **Biasing:** Integrated a current mirror at the tail to ensure a constant and stable bias current throughout the circuit.
* **Unity Gain Buffer (UGB):** Configured the amplifier in a negative feedback loop to evaluate its performance as a buffer, ensuring the inverting input correctly tracks the output.
* **Stability Analysis:** Characterized the frequency response to ensure the system remains stable across its operating range, achieving a robust phase margin.

## Analysis Included
* **DC Analysis:** Operating point verification and identification of the linear input/output range.
* **Transient Response:** Detailed step response analysis to calculate settling time and observe the system's dynamic stability.
* **Frequency Analysis (Bode Plot):** Magnitude and phase characterization using AC simulation (up to 10GHz) to determine gain and phase margins.
* **Slew Rate Measurement:** Evaluation of the maximum rate of change of the output voltage.

## Documentation
For a detailed technical breakdown, including schematics, simulation setups, and full result analysis, please refer to the project report:
* [**Differential to Single Ended Op Amp.pdf**](./Differential to Single Ended Op Amp.pdf)

## Tools Used
* **Cadence Virtuoso** – Schematic Editor.
* **Spectre / Maestro** – Simulation Engine.
* **ViVA / Calculator** – Signal Analysis and Waveform Visualization.
