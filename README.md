# DeepRL

A comprehensive collection of deep reinforcement learning algorithm implementations and experiments. This repository covers a wide range of methods, including value-based (DDQN, SARSA/QL, Dyna-Q), policy-gradient (PPO, REINFORCE), actor-critic, model-based (MPC), planning (MCTS), and advanced topics like Multi-Agent RL, Imitation Learning, and Meta-RL.

## Overview

This repository is designed as a hands-on resource for learning and experimenting with deep reinforcement learning (DeepRL). It contains several implementations and experiments demonstrating how different RL algorithms perform on various tasks. Each folder in the repository corresponds to a specific algorithm or a comparative study.


## Directory Structure 

This section provides a complete listing and thorough description of all the major directories and standalone files within the repository.

| Directory/File         | Description                                                                                                                                                                                  |
| :--------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **DDQN/**              | Implementation of the **Deep Double Q-Network**. This enhanced version of DQN uses two separate Q-networks to reduce overestimation bias, leading to more stable learning.                   |
| **Dyna_Q/**            | Code for the **Dyna-Q** algorithm. It integrates **planning** (using an environment model) with **direct reinforcement learning** (learning from experience) to accelerate convergence.      |
| **Imitation/**         | Contains algorithms for **Imitation Learning** (e.g., Behavior Cloning), where an agent learns a policy by mimicking actions from an expert's demonstration dataset.                         |
| **MCTS/**              | Implementation of the **Monte Carlo Tree Search** algorithm. MCTS is a powerful best-first search technique used for complex planning and decision-making by leveraging random simulations.  |
| **MPC/**               | Code for **Model Predictive Control**. This model-based technique uses a dynamic environment model to plan an optimal sequence of actions over a short, finite horizon at every step.        |
| **Multi Agent/**       | Experiments and implementations dedicated to **Multi-Agent Reinforcement Learning (MARL)**, exploring scenarios where multiple agents interact and coordinate within a shared environment.   |
| **PPO/**               | Implementation of **Proximal Policy Optimization**. A stable and high-performing policy gradient method that uses a clipped objective function to constrain policy updates.                  |
| **REINFORCE/**         | Implementation of the basic **REINFORCE** (Monte Carlo Policy Gradient) algorithm, a foundational policy gradient method.                                                                    |
| **SACvsDDPG/**         | A comparative study between **Soft Actor-Critic (SAC)** and **Deep Deterministic Policy Gradient (DDPG)**, highlighting SAC's stability and exploration benefits.                            |
| **SARSA_QL/**          | Implementations of classic off-policy **Q-Learning** and on-policy **SARSA** algorithms, serving as foundational value-based RL examples.                                                    |
| **Stable-Baselines3/** | Examples and utility scripts demonstrating the usage of the popular **Stable-Baselines3** framework for rapid prototyping and benchmarking.                                                  |
| `ConservativeQL.ipynb` | A Jupyter Notebook exploring **Conservative Q-Learning (CQL)**, an algorithm for **Offline Reinforcement Learning** that conservatively estimates Q-values to mitigate extrapolation errors. |
| `MetaRL.ipynb`         | A Jupyter Notebook demonstrating concepts and algorithms related to **Meta-Reinforcement Learning** (learning to learn), enabling agents to quickly adapt to new tasks.                      |
| `LICENSE`              | The repository's license file, detailing the terms of use.                                                                                                                                   |



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
