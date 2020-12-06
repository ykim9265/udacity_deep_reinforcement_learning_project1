
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
1. Create a python version 3.6 virtual environment.
2. For the environment, issue the following statements to install required dependencies:

Here is the command:

    pip install numpy matplotlib jupyter torch unityagents

If using `conda`, one can isssue the following command:

    conda create -n myenv python=3.6 numpy matplotlib jupyter torch
    conda activate myenv
    pip install unityagents

Note that I could not install `unityagents` in python3.7, but was able to in python3.6.

### Unity Environment

1. Clone the DRLND Repository

2. Download the Unity Environment

3. Step 3: Explore the Environment

If the Unity environment has been set up correctly, then the notebook TEST should run as shown below in the video:
https://www.youtube.com/watch?v=ltz2GhFv04A

## Instructions

To run the trained agent for the Banana environment, you can run the jupyter notebook TBD in the python environment that you created above.


