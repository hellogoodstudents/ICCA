# ICCA
ICCA: Independent multi-agent algorithm for distributed jamming scheduling
The ICCA Algorithm Designed in This Paper
Python Integrated Development Environment (IDE) Version:
PyCharm 2023.2.1 (Professional Edition)
Runtime Version: 17.0.8+7-b1000.8 amd64
Third-Party Libraries Used: anaconda_depends_2023.09 and PyTorch 1.13.1
Drawing programs for Figure 4 (Scenario 1), Figure 5 (Scenario 2), and Figure 6 (Scenario 3) have been added, which can generate images directly after execution.
In each scenario file:
Open main.py and click "Run" to execute the algorithm once with default settings. Modify the number of runs at the end of the program to enable repeated execution.
generate_nodes.py is the simulation program for Algorithm 1.
modify_communication_nodes.py is the simulation program for Algorithm 2.
jammer_first_run.py is the jamming program for the jammer’s first decision based on the proposed strategy.
jammer_run.py is the jamming program for the jammer’s non-first decisions based on the proposed strategy.
test.py is the detection program for jamming effectiveness in the simulation scenario.
A random number seed is set to ensure reproducibility.
Outputs communication_data.txt, which records the state information of each communication node in the simulation scenario after each jammer’s decision. The data fields are as follows (in order): communication node ID, communication node type, x-coordinate, y-coordinate, z-coordinate, electromagnetic environment noise at the node, transmit power of the communication node, maximum received power of the communication signal at the node, and sum of communication jamming signals at the node.
Outputs communication_interference_data.txt, which records the state information of each jammer in the simulation scenario after each jammer’s decision. The data fields are as follows (in order): jammer ID, jammer type, x-coordinate, y-coordinate, z-coordinate, electromagnetic environment noise at the node, jamming power of the jammer, and remaining battery capacity of the jammer.
Click to run the "Data Statistics" program to calculate the comparative data presented in the paper.
Click to run the files "Jammer Transmit Power Statistics.py", "JSR Average Line Chart.py", "Communication Node Transmit Power Heatmap.py", and "Communication Node JSR Heatmap.py" to generate corresponding images based on the results of a single experiment.
