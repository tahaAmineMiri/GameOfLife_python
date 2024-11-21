# GameOfLife_python

## Overview

This project implements Conway's Game of Life in Python. The Game of Life is a cellular automaton devised by the British mathematician John Horton Conway in 1970. It is a zero-player game, meaning that its evolution is determined by its initial state, requiring no further input. One interacts with the Game of Life by creating an initial configuration and observing how it evolves.

## Installation

To run this project, you need to have Python installed on your machine. Additionally, you need to install the following Python libraries:

- `matplotlib`
- `numpy`

You can install these libraries using pip:

```
pip install matplotlib numpy
```

## Usage

### Class: `GameOfLife`

The `GameOfLife` class implements the Game of Life. It provides methods to initialize the game grid, populate it with live cells, advance the game by one or more steps, and visualize the grid.

#### Methods

- `__init__(self, x_dim, y_dim)`: Initializes a new instance of the GameOfLife class with a grid of given dimensions.
  - **Parameters:**
    - `x_dim`: The number of rows in the grid.
    - `y_dim`: The number of columns in the grid.

- `get_grid(self)`: Gets the current state of the life grid.
  - **Returns:** The current state of the life grid.

- `print_grid(self)`: Prints the current state of the life grid in a readable format.

- `populate_grid(self, coord)`: Populates the game grid with live cells at the specified coordinates.
  - **Parameters:**
    - `coord`: A list of tuples. Each tuple represents the (x, y) coordinates of a live cell.
  - **Returns:** The updated life_grid with the new live cells.

- `make_step(self)`: Advances the game by one step according to the rules of the Game of Life.
  - **Returns:** The updated life_grid after one step.

- `make_n_steps(self, n)`: Advances the game by a specified number of steps.
  - **Parameters:**
    - `n`: The number of steps to advance the game by.
  - **Returns:** The updated life_grid after n steps.

- `draw_grid(self)`: Visualizes the current state of the game grid using a scatter plot.