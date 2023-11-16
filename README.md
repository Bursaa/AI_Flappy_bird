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

