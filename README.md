# Pipeline Test Bench Dataset

This repository contains data collected from a liquid pipeline transportation test bench. The dataset includes various experimental conditions and is intended for research in pipeline system analysis, fault detection, and hydraulic system behavior under different operating conditions.

## Dataset Overview
The dataset includes data from experiments conducted on a pipeline system, designed to simulate different fluid flow scenarios and study pipeline leakage, pressure, and flow conditions. The test bench system includes sensors for flow, vibration, and pressure, and can simulate a range of conditions such as:
- Pipeline leakage experiments
- Flow rate and fluid motion adjustments (steady-state and unsteady-state transportation)
- Liquid pipeline transportation conditions (straight pipes vs. bends, horizontal vs. vertical pipes)
- Pressure and flow conditions during pipeline blockages

The system features 8 centrifugal pumps, providing pipeline pressures ranging from 0.2 to 1.4 MPa, and is equipped with various sensors to monitor system performance.

## Data Structure
The data is organized in the following manner:
- `data/leakage/`: Contains data for leakage experiments, including flow, pressure, and vibration readings.
- `data/steady_state/`: Contains data from steady-state transportation experiments.
- `data/unsteady_state/`: Contains data from unsteady-state transportation experiments.
- `data/blockage/`: Contains data from experiments studying pressure and flow during pipeline blockages.

Each file contains sensor readings such as:
- Flow rate (m³/h)
- Pressure (MPa)
- Vibration data (if available)
- Control variables (such as valve opening degree)

## Key Parameters of the Pipeline Bench
- **Pipeline Material**: 304 Stainless Steel Pipe
- **Total Pipeline Length**: 144 m
- **Pipe Size**: DN40
- **Inner Diameter**: 42 mm
- **Wall Thickness**: 3 mm
- **Pump Number**: 8 centrifugal pumps forming 4 pump groups
- **Pressure Range**: 0.2–1.4 MPa

## How to Use the Data
You can download the data and load it using Python or MATLAB. Here is a simple example in Python to load a CSV file:

```python
import pandas as pd
data = pd.read_csv("path_to_your_data_file.csv")


## License
This dataset is licensed under the [MIT License](LICENSE).
