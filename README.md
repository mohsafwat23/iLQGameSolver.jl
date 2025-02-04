[![CI](https://github.com/itsahmedkhalil/iLQGameSolver.jl/actions/workflows/CI.yml/badge.svg)](https://github.com/itsahmedkhalil/iLQGameSolver.jl/actions/workflows/CI.yml)
[![codecov](https://codecov.io/gh/itsahmedkhalil/iLQGameSolver.jl/branch/main/graph/badge.svg?token=ZCZYZGCH2T)](https://codecov.io/gh/itsahmedkhalil/iLQGameSolver.jl)
# Iterative Linear-Quadratic Game Solver for Multi-Agent Nonlinear Robotic Interactions

This repo is inspired by [ilqgames](https://arxiv.org/abs/1909.04694), an efficient iterative linear-quadratic approximations for nonlinear multi-player general-sum differential games. 

It is still a work in progress. An example of a three point masses navigating at an intersection can be shown in the following GIF. 

![Alt Text](examples/assets/three_agent.gif)

## How to install for development

Open the Julia REPL, enter the package manager using `]`, and run the following command to clone the code
```bash
    dev https://github.com/itsahmedkhalil/iLQGameSolver.jl.git
```

A folder called iLQGameSolver should be created and it should contain the repo. Make changes and push your code.

## Todo list:

### Important:

- ~~Generalize for multiple agents:~~
    - ~~Pass the dynamics function manually. Looping over each agent is inefficient.~~ 

- Add documentation and write report

- ~~Receding horizon for online trajectory optimization~~
- Make tests for receeding horizon solver

- Make a better GUI for the results
  - Graphical representation of the robots pose and shape in plots
  - Add TurtleBot to MeshCat or on ROS to visualize results

-  ~~Put code in .jl file instead of .ipynb~~

- ~~Integrate the linear approximation of the nonlinear dynamics for multiple agents (linearize and discretize)~~
    - ~~Check that the point mass works using both dynamics~~

- ~~Use differential drive kinematics to use on TurtleBots~~

- Check augmented lagrangian dynamic programming for equality and inequality constraints

- Monte Carlo simulations to observe Nash Equilibria solutions

### Not important:
- Add state constraints

- Make cost functions user specified (not Qs and Rs)

- Test cost functions with analytic Hessians and gradients
