# UAV-TOP-Datasets

## Datasets for "Combining the A* Algorithm with Neural Networks to Solve the TOP with Obstacles and Environmental Factors"

This repository contains the benchmark datasets used in our research on solving the Team Orienteering Problem (TOP) with unmanned aerial vehicles (UAVs) in environments with obstacles and environmental factors.

### Paper Abstract

This paper addresses the team orienteering problem applied to unmanned aerial vehicles (UAVs), considering obstacle avoidance and environmental factors such as wind conditions and payload weight. The objective is to optimize UAV routes to maximize collected rewards while adhering to operational constraints. To achieve this, we first employ the A* algorithm for path planning, ensuring UAVs navigate efficiently while avoiding obstacles in a 2D grid-based environment. Then, a feedforward neural network estimates travel time based on UAV speed, wind conditions, trajectory distance, and payload weight. This estimation is incorporated into the optimization process to improve route planning accuracy. Numerical experiments evaluate the impact of various parameters, including obstacle placement, UAV speed, wind conditions, and payload weight. The results demonstrate the effectiveness of the proposed methodology in optimizing UAV routes under realistic constraints.

### Datasets

This repository includes two primary benchmark datasets used in our experimental evaluation:

#### Dataset 1: 21-node instance
- 21 nodes total (including start and finish depots)
- Grid size: 30×30 km
- Fleet: 2 UAVs
- Node distribution: Nodes distributed across the operational area
- Reward values: Varying rewards associated with each node
- Start/finish depots: Node 1 (start) and Node 21 (finish)
- Two variants: with and without obstacles
- Maximum route duration tested: 36-50 minutes

#### Dataset 2: 31-node instance
- 31 nodes total (including start and finish depots)
- Grid size: 30×30 km
- Fleet: 3 UAVs
- Node distribution: Nodes distributed across the operational area
- Reward values: Different rewards associated with each node
- Start/finish depots: Node 1 (start) and Node 31 (finish)
- Two variants: with and without obstacles
- Maximum route duration tested: 50 minutes

### File Format

Each dataset is provided in text format with the following structure:
```
n;[number of nodes]
m;[number of UAVs]
tmax;[maximum route duration]
[x-coordinate];[y-coordinate];[reward]
...
```

The first three lines specify the problem parameters, followed by node information with each line containing the x-coordinate, y-coordinate, and associated reward. The first and last nodes serve as the depot (start and finish points) and have zero rewards.

### Citation

If you use these datasets in your research, please cite our paper:

```
Freixes, A., Panadero, J., Juan, A.A. & Serrat, C. (2025). Combining the A* Algorithm 
with Neural Networks to Solve the TOP with Obstacles and Environmental Factors. 
Algorithms, 1, 0. https://doi.org/[DOI]
```

### License

This dataset is provided under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

### Contact

For questions regarding the datasets or the associated research, please contact:
- Alfons Freixes (afreixes@euncet.com)
- Angel A. Juan (ajuanp@upv.es)
