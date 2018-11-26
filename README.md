# Continuous Control
Project #2 for Udacity Deep Reinforcement Learning course.

## Project Details

This project uses the Unity [Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) environment.

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

This project uses the distributed (second) version that contains 20 identical agents, each with its own copy of the environment. The environment is considered solved when the average (over the last 100 episodes) score across the agents is at least 30.

## Getting Started
To set up your python environment to run the code in this repository, follow the instructions below.

1. Create (and activate) a new environment with Python 3.6.

        - __Linux__ or __Mac__:
        ```bash
        conda create --name drlnd python=3.6
        source activate drlnd
        ```
        - __Windows__:
        ```bash
        conda create --name drlnd python=3.6
        activate drlnd
        ```

2. Clone the repository and navigate to the `python/` folder.  Then, install several dependencies.
```bash
git clone https://github.com/udacity/deep-reinforcement-learning.git
cd deep-reinforcement-learning/python
pip install .
```

3. Download the Reacher environment from one of the links below.  Select the environment that matches your operating system:

  - **_Version 2: Twenty (20) Agents_**
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)


4. Place the file in this directory, and unzip (or decompress) the file.

## Instructions
Running the code in the repository and training the agent is straightforward. The `Continuous_Control.ipynb` Jupyter notebook should be used to run the code in the repository and train the agent.

I trained the policy on a MacBook Pro. The policy is implemented using PyTorch and the model is trained on CPU (only).

The PPO algorithm was used to train the policy. See the [report file](file:///Report.pdf) for a detailed description of the model and the training process.
