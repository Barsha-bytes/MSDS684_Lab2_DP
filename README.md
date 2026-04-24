# Solving Finite MDPs with Dynamic Programming
**MSDS 684: Reinforcement Learning | Regis University**

## Project Overview
This project implements **Policy Iteration** and **Value Iteration** algorithms to solve a GridWorld Markov Decision Process (MDP). Using the **Bellman Equations**, we solve for optimal state-values and policies in both deterministic and stochastic (slippery) environments.

## Key Features
- **Transition Dynamics:** Direct extraction of $P(s', r | s, a)$ from Gymnasium's `FrozenLake-v1`.
- **Custom Visualizations:** Heatmaps for Value Functions and Quiver Plots for Optimal Policies.
- **Analysis:** Comparative study of convergence rates and computational efficiency between PI and VI.

## Results
### Value Function Heatmap
The heatmap below reveals how rewards propagate from the goal back to the starting state.
![Value Function](Value%20Iteration.png)

### Policy Quiver Plot
The arrows indicate the optimal actions learned by the agent.
![Policy Plot](Policy%20iteration.png)

## References
Sutton, R. S., & Barto, A. G. (2018). *Reinforcement learning: An introduction* (2nd ed.). MIT Press.
