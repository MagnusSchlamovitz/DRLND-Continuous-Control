# DRLND-Continuous-Control
Continuous Control Project

[//]: # (Image References)

For this project, I will work with the Reacher environment.

![Trained Agents](./images/scene.png)


## The Environment

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of my agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

## Dependencies

This is an amended version of the python/ folder from the [ML-Agents repository](https://github.com/Unity-Technologies/ml-agents). It has been edited to include a few additional pip packages needed for the Deep Reinforcement Learning Nanodegree program.

Follow the instructions below to explore the environment on your own machine! You will also learn how to use the Python API to control your agent.

### Step 1: Activate the Environment

## Run the notebook

1. Execute in terminal `jupyter notebook Continuous_Control.ipynb` to load the notebook. Make sure that *ddpg_agent.py* and *model.py* are in the same folder.

2. Before running code in the notebook, change the kernel to match the `drlnd` environment by using the drop-down `Kernel` menu. 

  ![Kernel][image2]

3. To train the Agent execute:
  - Sections 1. Start the Environment
  - Section 2. Examine the State and Action Spaces
  - Section 3. Train the Agent with DDPG 
  
4. To watch a Smart Agent execute:
  - Sections 1. Start the Environment
  - Section 4. Watch a Smart Agent!


## References

* The Udacity's [Deep Reinforcement Learning Nanodegree program](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893) repository, https://github.com/udacity/deep-reinforcement-learning

* Lillicrap T.P., Hunt J.J., Pritzel A., et.al., Continuous control with deep reinforcement learning, arXiv:1509.02971v5, https://arxiv.org/abs/1509.02971

* Implementations of the **Deep Deterministic Policy Gradients** in OpenAI Gym environments:
    - [Pendulum](https://github.com/udacity/deep-reinforcement-learning/tree/master/ddpg-pendulum): Use OpenAI Gym's Pendulum environment.
    - [BipedalWalker](https://github.com/udacity/deep-reinforcement-learning/tree/master/ddpg-bipedal): Use OpenAI Gym's BipedalWalker environment.

* [Cheatsheet](https://github.com/udacity/deep-reinforcement-learning/blob/master/cheatsheet) for reinforcement learning.
