[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135623-e770e354-7d12-11e8-998d-29fc74429ca2.gif "Trained Agent"
[image2]: https://user-images.githubusercontent.com/10624937/42135622-e55fb586-7d12-11e8-8a54-3c31da15a90a.gif "Soccer"


# Project 3: Collaboration and Competition - Multi-Agent Deep Deterministic Policy Gradient (MADDPG) - Tennis Environment

## Introduction

For this project, you will work with the [Tennis](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#tennis) environment.

![Trained Agent][image1]

## Project Overview

This project involves training two agents in the Unity ML-Agents Tennis environment using the Multi-Agent Deep Deterministic Policy Gradient (MADDPG) algorithm. The goal of the agents is to keep a ball in play by hitting it over a net. The environment is considered solved when the agents achieve an average score of +0.5 over 100 consecutive episodes.

## Dependencies

To run this project, you'll need the following dependencies:

- Python 3.6+
- Unity ML-Agents
- PyTorch
- NumPy


## Getting Started

1. Clone the repository:

```bash
git clone https://github.com/akocabas/deep-reinforcement-learning.git
cd p3_collab-compet
```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

4. Place the file in the DRLND GitHub repository, in the `p3_collab-compet/` folder, and unzip (or decompress) the file. 


## 3. Train the Agents:

You can train the agents by running the Tennis.ipynb notebook


## 4. Test the Agents:

After training, you can test the trained agents by running the Tennis_test.ipynb notebook


This will load the saved networks and display the agents' performance in the environment.

## Files in the Repository

- Tennis_test.ipynb: Script to train the agents.
- Tennis_test.ipynb: Script to test the trained agents.
- `README.md`: Project overview and setup instructions.
- `REPORT.md`: Detailed report on the project, methodology, and results.

## Results

The trained agents were able to achieve an average score of 0.5, indicating successful learning.

