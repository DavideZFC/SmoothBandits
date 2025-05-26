# SmoothBandits

SmoothBandits is a Python project that implements continuous armed bandit algorithms. The environments are given by a smooth reward function which is accessible trough noisy observations.
In the continuous bandit problem, the algorithm cannot try all the arms even once, so that it has to exploit some notion of regularity of the function $f$ in order to discard arms without pulling them. In the continuous bandit literature, mainly two families of methods were introduced, depending on the type of assumptions on $f$.1) Lipschitzness: under the assumption that $f$ is Lipschitz or H\"older continuous, algorithm based on discretization were used. 2) RKHS representation: under the assumption that $f$ belongs to a reproducing kernel Hilbert space with known kernel, it is possible to solve the problem with kernel methods, and in particular Gaussian processes.
In this repo, we explore a strategy that reduces the problem to a standard linear bandit by approximating the space of smooth functions with the span of a basis endowed with a specific approximation property (Fourier features or polynomials).

to run a simple experiment:
`python prova.py`

## Project Structure

- `classes/`: Contains the main class definitions used in the project.
- `functions/`: Includes auxiliary functions and utilities to support the implementation of the algorithms.
- `prova.py`: Example or test script to demonstrate the use of the implemented classes and functions.
- `.gitignore`: Specifies files and directories to be ignored by version control.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/DavideZFC/SmoothBandits.git
