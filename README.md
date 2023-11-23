# RL-TrafficLight-Control-Adaptive-Traffic-Management
_This GitHub repo hosts an RL-based Traffic Light Control System (TLCS) for optimizing intersections. Employing Reinforcement Learning, it adapts signal timings in real-time, reducing congestion and enhancing traffic efficiency._ 

- **Normal Traffic Simulation**
    > ![R1(Normal)](https://github.com/Saumyadeepm/RL-TrafficLight-Control-Adaptive-Traffic-Management/assets/100332918/50a5b852-ff4d-4cd9-99a3-192da41bab2f)
<br />

- **Traffic Simulation By Accumulated Waiting Time**
    > ![R2 (By Accumulated Waiting Time)](https://github.com/Saumyadeepm/RL-TrafficLight-Control-Adaptive-Traffic-Management/assets/100332918/614f1f14-0264-489f-b052-b48b086045fc)
<br />

- **Traffic Simulation On the Basis of Direction They Are Coming From**
    > ![R3 (On the Basis of Direction They Are Coming From)](https://github.com/Saumyadeepm/RL-TrafficLight-Control-Adaptive-Traffic-Management/assets/100332918/09aaffab-2a2e-448e-9f00-2d9d36f8afe3)
<br />

- **Traffic Simulation On The Basis of Braking Gap**
    > ![R4 (On the Basis of Braking Gap)](https://github.com/Saumyadeepm/RL-TrafficLight-Control-Adaptive-Traffic-Management/assets/100332918/0004f13b-b469-4193-8868-1750ee585a9b)
<br />

## Overview


The project comprises several modules:

- **Training Simulation:** Contains the main simulation loop for training the reinforcement learning model.
- **Generator:** Generates traffic scenarios for simulation episodes.
- **Memory:** Implements the memory buffer for storing and sampling experiences.
- **Model:** Includes classes for training, testing, and saving/loading the neural network model.
- **Visualization:** Provides functions to visualize performance metrics during and after training.
- **Utils:** Contains utility functions for configuration, SUMO integration, and path handling.

## Installation

To run the project, follow these steps:

1. Clone this repository:

    ```bash
    git clone "https://github.com/Saumyadeepm/RL-TrafficLight-Control-Adaptive-Traffic-Management"
    cd rl_traffic_simulation_project
    ```

2. Install the necessary dependencies:
    - Installing SUMO
      ```bash
      !add-apt-repository ppa:sumo/stable -y
      !apt-get update -y
      !apt-get install sumo sumo-tools sumo-doc
      ```
    - Installing Traci
      ```bash
      !pip install traci
      ```

## Usage

### Training

1. Configure training settings in `training_settings.ini`.
2. Run the training simulation:

    ```bash
    python training_main.py
    ```

### Testing

1. Set up the testing configuration in `testing_settings.ini`.
2. Perform model testing:

    ```bash
    python testing_main.py
    ```
## Contributing
_Contributions are welcome. Feel free to open issues or submit pull requests if you have any suggestions or improvements._
Created By [Saumyadeep Mitra](https://in.linkedin.com/in/saumyadeep-mitra-a64030236)


## License
_This project is open-source and released under the_ [MIT License](https://opensource.org/licenses/MIT)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
