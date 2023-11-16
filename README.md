# Flappy Bird with NEAT

The classic game of Flappy Bird implemented using Python and Pygame, trained using NEAT (NeuroEvolution of Augmenting Topologies) for AI gameplay.

## Overview

This project includes a Python implementation of the Flappy Bird game using Pygame and an AI agent trained with the NEAT algorithm to play the game autonomously. The AI agent learns to navigate through pipes by evolving neural networks that control the bird's actions.

## Features

- Pixel-perfect collision using masks for accurate gameplay interaction.
- NEAT algorithm implementation for evolutionary learning in the game.
- Visualized statistics and neural network architecture.

## Configuration File

The `config-feedforward.txt` file contains parameters and settings for the NEAT algorithm used in training the neural networks. Modify this file to tweak various algorithmic parameters for evolving better AI agents.

### Requirements

To set up the project, ensure you have the required Python libraries installed. Use the following command to install dependencies:

```bash
pip install -r requirements.txt
```

## Usage

### Training 

To make training start:

```bash
python flappy_bird.py
```

### Configuration

The configuration file `config-feedforward.txt` includes settings for the NEAT algorithm, defining parameters like population size, mutation rates, and species threshold.

**Adjusting Parameters:**

To modify the NEAT algorithm's behavior, update the values in the `config-feedforward.txt` file:

- `population_size`: Defines the number of birds in each generation.
- `mutation_rate`: Controls the likelihood of genetic mutation in the algorithm.
- `compatibility_threshold`: Sets the threshold for species compatibility in the algorithm.

### Evaluation

The AI agent's fitness is determined based on its performance in the game. The algorithm trains the agent to maximize its fitness score, improving its ability to play Flappy Bird.

**Training Process:**

- The algorithm progresses through multiple generations, evolving neural networks for the bird population.
- Fitness is calculated based on the bird's ability to navigate and survive through pipes.
- Higher fitness correlates with better performance in the game.
- The trained neural network (`best.pickle`) represents the best-performing network achieved after training.

**Output:**

- Once training completes, the best-performing neural network (`best.pickle`) is available for use.
- This trained network can be loaded and used to play Flappy Bird without further training.

## Files Included

- `flappy_bird.py`: Main Python script containing the game implementation and NEAT training.
- `config-feedforward.txt`: Configuration file for the NEAT algorithm.
- `requirements.txt`: List of required Python packages and their versions.

## Acknowledgments

- This project was inspired by the classic Flappy Bird game.
- NEAT algorithm implementation reference: [NEAT-Python](https://neat-python.readthedocs.io/en/latest/)


