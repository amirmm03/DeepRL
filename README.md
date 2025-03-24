# DeepRL

A collection of deep reinforcement learning algorithm implementations. This repository includes various methods such as Deep Double Q-Network (DDQN), Proximal Policy Optimization (PPO), REINFORCE, comparisons like SAC vs DDPG, SARSA/QL, and examples using Stable Baselines3.

## Overview

This repository is designed as a hands-on resource for learning and experimenting with deep reinforcement learning (DeepRL). It contains several implementations and experiments demonstrating how different RL algorithms perform on various tasks. Each folder in the repository corresponds to a specific algorithm or a comparative study.

## Directory Structure

- **DDQN/** - Implementation of the Deep Double Q-Network algorithm.
- **PPO/** - Code for Proximal Policy Optimization.
- **REINFORCE/** - Implementation of the REINFORCE algorithm.
- **SACvsDDPG/** - Comparative study between Soft Actor-Critic (SAC) and Deep Deterministic Policy Gradient (DDPG).
- **SARSA_QL/** - Implementations of SARSA and Q-Learning.
- **Stable-Baselines3/** - Examples using the Stable-Baselines3 framework.
- **LICENSE** - The repository is licensed under the Apache-2.0 license.

## Requirements

- Python 3.8 or above
- [NumPy](https://numpy.org/)
- [PyTorch](https://pytorch.org/) or [TensorFlow](https://www.tensorflow.org/) (depending on the implementation)
- [Gym](https://github.com/openai/gym) for simulation environments
- [Stable-Baselines3](https://github.com/DLR-RM/stable-baselines3) (for relevant examples)

## Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/amirmm03/DeepRL.git
   cd DeepRL
   ```

2. **Create a virtual environment (optional but recommended):**
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the required packages:**
   ```bash
   pip install -r requirements.txt
   ```
   If `requirements.txt` is missing, manually install:
   ```bash
   pip install numpy gym torch stable-baselines3
   ```

## Usage

Each folder contains its own example or experiment:

- **Run an experiment:**  
  Navigate to the corresponding folder and execute the main script. Example:
  ```bash
  cd DDQN
  python ddqn_main.py
  ```

- **For Jupyter Notebooks:**  
  Start Jupyter and open the relevant notebook:
  ```bash
  jupyter notebook
  ```

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests. Follow the existing code style and include appropriate tests.

## License

This project is licensed under the [Apache-2.0 License](./LICENSE).
