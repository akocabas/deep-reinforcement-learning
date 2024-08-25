[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/43851024-320ba930-9aff-11e8-8493-ee547c6af349.gif "Trained Agent"
[image2]: https://user-images.githubusercontent.com/10624937/43851646-d899bf20-9b00-11e8-858c-29b5c2c94ccc.png "Crawler"


# Project 2: Continuous Control - Deep Deterministic Policy Gradient (DDPG)

This repository contains an implementation of the Deep Deterministic Policy Gradient (DDPG) algorithm to solve a continuous control problem in a Unity ML-Agents environment.

## Project Overview

The goal of this project is to train an agent to control a double-jointed arm to reach a target location. The environment is provided by Unity's Reacher environment, where the agent receives a reward for keeping the end-effector of the arm in the target location for as long as possible.


## Getting Started

### Prerequisites

- Python 3.6+
- PyTorch
- Unity ML-Agents
- Additional libraries as listed in `requirements.txt`

### Installation

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
	

2. If running in **Windows**, ensure you have the "Build Tools for Visual Studio 2019" installed from this [site](https://visualstudio.microsoft.com/downloads/).  This [article](https://towardsdatascience.com/how-to-install-openai-gym-in-a-windows-environment-338969e24d30) may also be very helpful.  This was confirmed to work in Windows 10 Home.  

3. Follow the instructions in [this repository](https://github.com/openai/gym) to perform a minimal install of OpenAI gym.  
	- Next, install the **classic control** environment group by following the instructions [here](https://github.com/openai/gym#classic-control).
	- Then, install the **box2d** environment group by following the instructions [here](https://github.com/openai/gym#box2d).
	
4. Clone the repository (if you haven't already!), and navigate to the `python/` folder.  Then, install several dependencies.  
    ```bash
    git clone https://github.com/akocabas/deep-reinforcement-learning
    cd deep-reinforcement-learning/python
    pip install .
    ```

5. Create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `drlnd` environment.    
    ```bash
    python -m ipykernel install --user --name drlnd --display-name "drlnd"
    ```

6. Before running code in a notebook, change the kernel to match the `drlnd` environment by using the drop-down `Kernel` menu. 


7. Go to p2_continuous-control:
    ```bash
    cd p2_continuous-control
    ```

8. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

9. Download the Unity Environment:
    - Download the appropriate environment for your operating syste
    - - **_Version 1: One (1) Agent_**
        - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
        - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
        - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)
        - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)

### Running the Code

To train the agent:

1. Open the Jupyter Notebook `Continuous_Control.ipynb`.
2. Run the cells in the notebook to start the training process.
3. The agent will interact with the environment, and training progress will be displayed, including the average score over 100 episodes.

To test the trained agent:

1. Ensure that the trained model weights are available (saved as `checkpoint_actor.pth` and `checkpoint_critic.pth`).
2. Load the model weights and run the agent in the environment by running Continuous_Control_test.ipynb to observe its performance.

### Files in the Repository

- `Continuous_Control.ipynb`: Jupyter Notebook containing the code to train the DDPG agent.
- `Continuous_Control_test.ipynb`: Jupyter Notebook containing the code to test the DDPG agent.
- `ddpg_agent.py`: Contains the implementation of the DDPG agent, including the Actor and Critic networks.
- `model.py`: Defines the neural network architectures for the Actor and Critic.
- `checkpoint_actor.pth`: Saved model weights for the actor network.
- `checkpoint_critic.pth`: Saved model weights for the critic network.
- `README.md`: This file, containing an overview of the project and instructions for use.
- `REPORT.md`: A report detailing the implementation and results.

## Results

The agent successfully solved the environment, achieving an average score of over 30 within ca. 300 episodes. See `REPORT.md` for a detailed analysis.
