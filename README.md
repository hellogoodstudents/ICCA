# ICCA: Independent Multi-agent Algorithm for Distributed Jamming Scheduling
This repository provides the official Python implementation of the ICCA (Independent multi-agent algorithm for distributed jamming scheduling) algorithm.

## Environment Requirements
- IDE: PyCharm 2023.2.1 (Professional Edition)
- Python Runtime: 17.0.8+7-b1000.8 amd64
- Dependencies: 
  - anaconda_depends_2023.09
  - PyTorch 1.13.1

## Code Structure & Execution Guide
### Core Algorithm Files
| File Name                  | Function Description                                                                 |
|----------------------------|--------------------------------------------------------------------------------------|
| generate_nodes.py          | Simulation implementation for Algorithm 1 (node generation logic)                    |
| modify_communication_nodes.py | Simulation implementation for Algorithm 2 (communication node modification logic)  |
| jammer_first_run.py        | Jammer's first decision-making program based on ICCA strategy                       |
| jammer_run.py              | Jammer's non-first decision-making program based on ICCA strategy                   |
| test.py                    | Jamming effectiveness detection program in simulation scenarios                     |

### Execution Steps
1. Open the target scenario folder, run `main.py` to execute the ICCA algorithm once with default settings.
2. Modify the "number of runs" parameter at the end of `main.py` to enable repeated execution.
3. Set random number seed is fixed to ensure experimental reproducibility.

### Output Files
- `communication_data.txt`: Records state information of each communication node after each jammer's decision (fields: node ID, type, x/y/z coordinates, electromagnetic noise, transmit power, max received power, sum of jamming signals).
- `communication_interference_data.txt`: Records state information of each jammer after each decision (fields: jammer ID, type, x/y/z coordinates, electromagnetic noise, jamming power, remaining battery capacity).

### Data Visualization & Statistics
Run the following scripts to generate experimental results visualization (consistent with the algorithm's performance analysis):
- `Jammer Transmit Power Statistics.py`: Statistics of jammer transmit power
- `JSR Average Line Chart.py`: Average JSR (Jamming-to-Signal Ratio) line chart
- `Communication Node Transmit Power Heatmap.py`: Heatmap of communication node transmit power
- `Communication Node JSR Heatmap.py`: Heatmap of communication node JSR
- `Data Statistics.py`: Calculates comparative performance data of the ICCA algorithm
