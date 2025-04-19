# Pipeline Test Bench Dataset

This repository contains data collected from a liquid pipeline transportation test bench. The dataset includes various experimental conditions and is intended for research in pipeline system analysis, fault detection, and hydraulic system behavior under different operating conditions.
## Dataset Overview
The dataset includes data from experiments conducted on a pipeline system under different operating conditions. The system consists of various sensors such as flow, pressure, and vibration sensors to monitor the pipeline's operational status. A comprehensive inspection is carried out before the experiments to ensure no leakage occurs and that all sensors are functioning and calibrated correctly.

The experimental scheme includes five distinct operating conditions corresponding to the operation of the pipeline with one to five pumps activated. For each condition:
- The data collection lasts for 10 minutes.
- The sampling rate is set at 10 Hz.
- Electromagnetic flow sensors are installed at both the inlet and outlet positions of the pipeline.
- Two pressure sensors and four vibration sensors are mounted on the pipeline surface.

The data collected includes:
- Four vibration sensors
- Two pressure sensors
- Two flow sensors

## Data Structure
The data is organized in the following manner:
- `data/pump_condition/`: Contains data from experiments under different pump operating conditions, with five pump scenarios corresponding to the operation of the pipeline with one pump, two pumps, three pumps, four pumps, and five pumps activated, respectively.
  - Files include: `1bengzc`, `2bengzc`, `3bengzc`, `4bengzc`, and `5bengzc`.
  - Each file contains sensor data collected during the operation of different pumps, including flow, pressure, vibration readings, and other relevant parameters.

## Experimental Setup
- **Flow Sensors**: Electromagnetic flow sensors are installed at both the inlet and outlet positions of the pipeline.
- **Pressure Sensors**: Two pressure sensors are used to monitor the pressure in the pipeline.
- **Vibration Sensors**: Four vibration sensors are mounted on the pipeline surface to measure vibration during pump activation.
- **Pump Configurations**: Data was collected under five different pump configurations, ranging from one pump to five pumps activated.
- **Sampling Rate**: 10 Hz.
- **Experiment Duration**: 10 minutes for each condition.
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

