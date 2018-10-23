# DRLND-Collaboration-and-Competition

## Collaboration and Competition Project
For this project, I will work with the [Tennis](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#tennis) environment.

![Trained Agents](./images/tennis.png)

## The Environment
In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping.

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.
This yields a single score for each episode.
The environment is considered solved, when the average (over 100 episodes) of those scores is at least +0.5.

## Dependencies
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

#### 2. Clone the repository (if you haven't already!), and navigate to the python/ folder. Then, install several dependencies.

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

- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)

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

1. Execute in terminal `jupyter notebook Tennis.ipynb` to load the notebook. Make sure that *agent.py* and *model.py* are in the same folder.

2. Before running code in the notebook, change the kernel to match the `drlnd` environment by using the drop-down `Kernel` menu. 


