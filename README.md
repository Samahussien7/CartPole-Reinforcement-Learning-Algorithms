# CartPole Reinforcement Learning Algorithms

## Description
This project implements three different reinforcement learning algorithms—Monte Carlo, Q-learning, and SARSA—on the classic CartPole problem.

### CartPole Environment
In the CartPole environment, a pole is attached by an un-actuated joint to a cart, which moves along a frictionless track. The pendulum starts upright, and the goal is to prevent it from falling over by increasing and reducing the cart's velocity.

### Source
This environment corresponds to the version of the CartPole problem described by Barto, Sutton, and Anderson.

### Actions
- **Type:** Discrete (2)
- **Actions:**
  - `0`: Push cart to the left
  - `1`: Push cart to the right

### Reward
- **Reward:** The agent receives a reward of 1 for every step taken, including the termination step.

### Episode Termination
- **Conditions:**
  1. Pole angle is more than ±12°.
  2. Cart position is more than ±2.4 (center of the cart reaches the edge of the display).
  3. Episode length is greater than 200 (500 for version 1).

### Solved Requirements
- The problem is considered solved when the average reward is greater than or equal to 195.0 over 100 consecutive trials.

## Implemented Algorithms

### 1. Monte Carlo
Monte Carlo methods are a class of algorithms that rely on repeated random sampling to obtain numerical results. In this project, Monte Carlo is used to estimate the value of each state-action pair by averaging the rewards received following visits to those pairs.


[MC-demo](https://github.com/user-attachments/assets/6a93d926-b52f-4a94-807d-92ddbb65e82f)



### 2. Q-learning
Q-learning is an off-policy learner. It seeks to find the best action to take given the current state. It learns the quality of actions, denoted as Q-values, which tells an agent what action to take under what circumstances.


[QL-demo](https://github.com/user-attachments/assets/e980203e-8acb-41ed-bf8a-e1144ef07ceb)



### 3. SARSA (State-Action-Reward-State-Action)
SARSA is an on-policy learning algorithm. It updates the Q-values using the action actually taken by the agent, making it more conservative compared to Q-learning.


[SARSA-demo](https://github.com/user-attachments/assets/9954090c-2856-4bac-89dd-31f3c7378f81)



## Installation
To run this project, you need to have Python and the following libraries installed:
- `gym`
- `numpy`

You can install the required libraries using the following command:
```bash
pip install gym numpy
```

## Acknowledgements
- This project is based on the CartPole problem as described by Barto, Sutton, and Anderson.
- The OpenAI Gym library is used for the CartPole environment.

## Contact
For any questions or issues, please open an issue on this repository or contact me.

