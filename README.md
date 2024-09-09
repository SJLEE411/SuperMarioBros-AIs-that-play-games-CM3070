# SuperMarioBros-AIs that play games CM3070
 

This project involves building and comparing two AI agents—**Kane** (Deep Q-Network with pre-programmed behavior) and **Abel** (Proximal Policy Optimization)—designed to play Super Mario Bros using OpenAI Gym and PyTorch. This README will guide you through setting up the environment, installing dependencies, and running the project.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dependencies](#dependencies)
3. [Installation](#installation)
4. [Running the Project](#running-the-project)
5. [Training the AI](#training-the-ai)
6. [Evaluation and Results](#evaluation-and-results)

---

## Project Overview

This repository contains two primary AI agents:

- **Kane**: Uses a Deep Q-Network (DQN) with pre-programmed behaviors such as a long jump to navigate the game.
- **Abel**: Uses Proximal Policy Optimization (PPO), a reinforcement learning algorithm, to learn and adapt to the environment.

The game environment is based on **Super Mario Bros** using the `gym-super-mario-bros` library, with agents developed using **PyTorch**.

---

## Dependencies

To run this project, you'll need the following dependencies:

- Python 3.8+
- `gym`: The OpenAI Gym library for creating and managing environments.
- `gym-super-mario-bros`: The custom Mario environment.
- `nes-py`: A Nintendo Entertainment System emulator for Python (required by `gym-super-mario-bros`).
- `torch`: The PyTorch deep learning library.
- `numpy`: For numerical computations.
- `opencv-python`: For image preprocessing.
- `matplotlib`: For plotting and visualization of metrics.
- `pip` for installing packages.

---

## Installation

Follow these steps to set up and run the project.

### Step 1: Clone the Repository

```bash
git clone https://github.com/SJLEE411/SuperMarioBros-AIs-that-play-games-CM3070.git
cd SuperMarioBros-AIs-that-play-games-CM3070
```

### Step 2: Create Virtual Environment

It is recommended to create a virtual environment to avoid conflixts with toehr python packages.
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### Step 3: Install Dependencies

You can install all the required dependencies using `pip`.

```bash
pip install gym
pip install gym-super-mario-bros
pip install nes-py
pip install torch
pip install numpy
pip install opencv-python
pip install matplotlib

```

Rest of installations will follow along with order of the cells. Excute notebook from top to bottom. or **Run all**.

## Running the Project

Make sure all dependencies are installed, and the environment is activated (if using a virtual environment).

Run the Jupyter notebooks provided in the repository:
- `Kane with DQN and preprogram.ipynb`
- `mario prototype - Abel.ipynb`


## Training the AI

In each notebook:

- **Kane**:Train the DQN agent with pre-programmed behavior
- **Abel**: Train the PPO agent to lean the game autonomously

Both notebooks include training loops, hyperparameter configs and logging of rewards,
losses, and actions.The models can be saved after training.

## Evaluation and Results

Once the models are trained, you can evaluate them by running the evaluation sections in each notebook. This will load the saved models and dimulate the agent playing the game collecting statistics such as:

- Total rewards per episode.
- Action distributions
- Performance comparisons between the two agents

As well as you can view PPO statistics with PPO's given localhost Tensorboard server as well as check the outputs as the changing expeirenced_variance or trained_loss on Abel.

For Kane, you can use pre made matplotlib cell to see the graphs after training.


Due to file constraint, train history of Abel was not uploaded here. Please check below google drive

https://drive.google.com/drive/folders/1RCJqtZxj80j0k377ymWmIYn6I2iLBttx?usp=sharing
