# Flappy Evolution: A NEAT-Powered Flappy Bird AI

This repository contains a **Flappy Bird** project powered by the **NEAT** (NeuroEvolution of Augmenting Topologies) algorithm. The AI (genomes) learns over successive generations to navigate through pipes without colliding, effectively mastering the game on its own!

## Overview

In this project, multiple bird agents attempt to dodge the pipes in a Flappy Bird environment. Each bird is controlled by a neural network whose weights (and structure, if NEAT is configured to allow that) evolve every generation. The fittest individuals (those who travel the farthest without crashing) pass on their “genes,” leading to increasingly better performance over time.

**Key Technologies Used**:

- **Python** (3.7+ recommended)
- **[Pygame](https://www.pygame.org/news)** for the game rendering, event handling, and collision detection.
- **[NEAT-Python](https://neat-python.readthedocs.io/en/latest/)** for the evolutionary algorithm that trains the neural networks.

---

## Features

- **Neural Network Control**: Each bird’s jumping behavior is determined by a simple feed-forward neural network.
- **Evolutionary Algorithm**: NEAT adjusts the weights (and optionally topology) of these networks based on a fitness function (the distance traveled).
- **Configurable Parameters**: Key parameters (e.g., population size, activation function, number of generations) can be tuned in `config-feedforward.txt`.
- **Real-Time Visualization**: Watch as the birds learn to navigate the game environment in real time.

---

## Installation

1. **Clone or Download this Repository**:
   ```bash
   git clone https://github.com/DivySolanki/Flappy-Evolution.git
   cd Flappy-Evolution
   ```
2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Game**:
   ```bash
   python main.py
   ```

Enjoy watching your own population of Flappy Bird agents evolve! If you have any questions, feel free to open an issue or contribute to the project.

Happy Flapping!
