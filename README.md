# Q-Learning Agent for Frozen Lake Environment

## Project Name: Q-Learning Agent for Frozen Lake

### Description
This project implements a **Q-Learning Agent** that learns to navigate through the **Frozen Lake** environment using the **Q-learning** reinforcement learning algorithm. The agent uses an **epsilon-greedy strategy** to explore the environment and update the Q-values based on the rewards it receives. The project also allows for **manual control** of the agent for comparison and testing purposes.

The Frozen Lake environment simulates a grid-like world where the agent must navigate to a goal while avoiding holes. The agent learns the optimal policy to reach the goal efficiently while avoiding hazards.

### Features
- **Q-Learning Agent**: The agent uses Q-learning to update its policy and improve its decision-making over time.
- **Epsilon-Greedy Exploration**: The agent balances exploration (random actions) and exploitation (greedy actions based on the current Q-values).
- **Training & Testing Modes**: The agent can be trained to learn the optimal policy and then tested using the learned model.
- **Manual Control Mode**: Users can manually control the agent to test different strategies or visualize the environment.
- **Model Saving & Loading**: The agent’s Q-table is saved after training and can be loaded for testing or further improvement.
  
### Dependencies
- **Python 3.x**
- **NumPy**: For numerical operations and Q-table management.
- **Pygame**: For visual rendering of the environment.
- **rl_base**: Contains the base classes and utilities for reinforcement learning agents.
- **envs.frozen_lake**: Implements the Frozen Lake environment.
- **gui.main_pygame**: Provides the main Pygame interface for visualizing the agent's actions and environment.
  
### How to Run

1. **Install Dependencies**:
   Install the required Python libraries using `pip`:
   ```
   pip install numpy pygame
   ```
2. **Run the Agent**:
   To train the Q-learning agent:
   ```
   python main.py --agent q_learning --mode train
   ```
   To test the trained Q-learning agent:
   ```
   python main.py --agent q_learning --mode test
   ```
   To control the agent manually:
   ```
   python main.py --agent manual --mode train
   ```
   
