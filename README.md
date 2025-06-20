# traveling-salesman-ga

# Genetic Algorithm for the Traveling Salesman Problem (TSP)

This repository contains a Python implementation of a **Genetic Algorithm (GA)** designed to solve the **Traveling Salesman Problem (TSP)**. The algorithm uses standard genetic operators such as selection, crossover, and mutation to evolve a population of candidate solutions.

---

## Features

- Reads TSP instances using the `tsplib95` library
- Fitness calculation based on total tour distance
- Mutation via city-swap
- Supports customizable GA parameters: population size, mutation rate, generations, etc.
- Jupyter Notebook interface for visualization and experimentation

---

## Problem Description

The **Traveling Salesman Problem (TSP)** is a classic optimization problem where the objective is to find the shortest possible route that visits a set of cities exactly once and returns to the origin city.

---

## Algorithm Overview

### Steps:
1. **Population Initialization**  
   Randomly generate a set of valid permutations (tours).

2. **Fitness Evaluation**  
   Compute the total distance of each tour using TSPLib distance data.

3. **Selection**  
   Select individuals for reproduction using methods like tournament selection.

4. **Crossover**  
   Combine parent tours to create offspring. Can be extended with PMX, OX, or k-point crossover.

5. **Mutation**  
   Swap two cities in a tour with a given probability to introduce variation.

6. **Survivor Selection**  
   Form the next generation from the fittest individuals.

7. **Termination**  
   Stop after a fixed number of generations or when improvement stagnates.

---

## File Structure

- `traveling-salesman-ga.ipynb` – Jupyter notebook containing the full implementation with explanations and examples

---

## Requirements

Install the required dependencies using pip:

```bash
pip install tsplib95
