# DRLND-Continuous-Control
Continuous Control Project

[//]: # (Image References)

For this project, I will work with the Reacher environment.

![Trained Agents](./images/reacher.gif)


## The Environment

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of my agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

## Dependencies

This is an amended version of the python/ folder from the [ML-Agents repository](https://github.com/Unity-Technologies/ml-agents). It has been edited to include a few additional pip packages needed for the Deep Reinforcement Learning Nanodegree program.


To set up your python environment to run the code in this repository, follow the instructions below.

#### 1. Create (and activate) a new environment with Python 3.6.

__Linux__ or __Mac:__
```bash
conda create --name drlnd python=3.6
source activate drlnd
```
	
__Windows:__
```bash
conda create --name drlnd python=3.6 
activate drlnd
```

#### 2. Clone the repository (if you haven't already), and navigate to the `python/` folder.  Then, install several dependencies.

```bash
git clone https://github.com/udacity/deep-reinforcement-learning.git
cd deep-reinforcement-learning/python
pip install .
```

#### 3. Create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `drlnd` environment.  
```bash
python -m ipykernel install --user --name drlnd --display-name "drlnd"
```

#### 4. Download the Unity Environment

You need only select the environment that matches your operating system:

__Version 1: One (1) Agent__

- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)


__Version 2: Twenty (20) Agents__

- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
- Windows (64-bit): [click here]()


This project uses rich simulation environments from [Unity ML-Agents](https://github.com/Unity-Technologies/ml-agents) but you will not need to install Unity - the environment is already built into the downloaded file.

#### 5. If you plan to play with the OpenAI gym examples, follow the instructions in [this repository](https://github.com/openai/gym):

- perform a minimal install of OpenAI gym:
```bash
git clone https://github.com/openai/gym.git
cd gym
pip install -e .
```    

- install the **classic control** environment group:
```bash
pip install -e '.[classic_control]'
```

- install the **box2d** environment group:
```bash
pip install -e '.[box2d]'
```

## Run the notebook

1. Execute in terminal `jupyter notebook Continuous_Control.ipynb` to load the notebook. Make sure that *ddpg_agent.py* and *model.py* are in the same folder.

2. Before running code in the notebook, change the kernel to match the `drlnd` environment by using the drop-down `Kernel` menu. 

  ![Kernel](./images/jupyter.PNG)
