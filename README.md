
# Overview

This repository contains my "Project 1" submission for Udacity's nanodegree program, "Deep Reinforcement Learning" started in late 2020.

It provides an implementation of a learning agent that solves the "Banana" environment.


# Project Details

In the "Banana" environment, an agent navigates a square world and collects bananas.

In terms of rewards, +1 and -1 are provided to the agent for collecting "yellow" and "blue" bananas, respectively.
The goal of the agent is to collect as many yellow bananas while avoiding blue ones.

The state space has 37 dimensions, containing the agent's velocity and "ray-based" perception
of objects around the agent's forward direction.
With this state information, the agent has to maximize total reward by selecting one of 4 actions.

The 4 available actions are as shown below:
- "0": Move forward
- "1": move backward
- "2": turn left
- "3": turn right

The task is episodic, meaning it has clear beginning and an end, and everything gets reset at the start of each episode.
In order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

Note that to run this Banana enviroment, the user has to use the provided Unity environment file, and *not* use the environment on the ML-agents GitHub page.


# Getting Started

## Installation
The following instructions have been tested on the linux ubuntu environment.

### Python virtual environment
1. Create a python version 3.6 virtual environment. You can use `conda` or `pyenv`.
2. Once you `activate` into the environment, issue the following statements to install required dependencies:

Here is the command:

    pip install numpy matplotlib jupyter torch unityagents

If using `conda`, one can isssue the following command:

    conda create -n myenv python=3.6 numpy matplotlib jupyter torch
    conda activate myenv
    pip install unityagents

Note that I could not install `unityagents` in python3.7, but was able to in python3.6.

### Unity Environment

#### 1. Download the Unity Environment

To run the notebook, you need to download one of the prepared Unity environment files matching your setup:

- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

The zip file needs to be placed in the root folder, and uncompressed.

#### 2. Explore the Environment

If the Unity environment has been set up correctly, then the notebook should 
run like the one shown below in the video: [click here](https://www.youtube.com/watch?v=ltz2GhFv04A)

## Instructions

To train an agent for the Banana environment, you can run the jupyter 
notebook `training_code.ipynb` in the python environment that you created above.


