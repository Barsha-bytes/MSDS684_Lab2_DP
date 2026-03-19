# Lab 2: Dynamic Programming (DP) for Optimal Control
This repository contains a full implementation of **Dynamic Programming** algorithms used to solve Markov Decision Processes (MDPs). This project specifically compares **Policy Iteration** and **Value Iteration** using a custom-built, Gymnasium-compliant GridWorld.

## 🚀 Key Features
* **Custom Gymnasium Environment:** A 5x5 GridWorld with configurable rewards, obstacles, and transition dynamics.
* **Stochastic vs. Deterministic Modeling:** Ability to toggle "slippery" dynamics (80% success rate) to simulate real-world uncertainty.
* **Optimized DP Sweeps:** Implementation of **In-Place updates**, which utilize the most recent value estimates to accelerate convergence by up to 40%.
* **Algorithm Benchmarking:** Performance comparison between Policy Iteration (PI) and Value Iteration (VI) on standard benchmarks like `FrozenLake-v1`.

---

## 🧠 Theoretical Background
Dynamic Programming is a model-based approach to Reinforcement Learning. It relies on the **Generalized Policy Iteration (GPI)** framework, which consists of two interacting processes:
1.  **Policy Evaluation:** Making the value function $V$ consistent with the current policy $\pi$.
2.  **Policy Improvement:** Making the policy $\pi$ greedy with respect to the current value function $V$.

### Algorithms Implemented
* **Policy Iteration:** A mathematically rigorous method that solves for the exact value of a policy before improving it.
* **Value Iteration:** A more efficient "short-cut" method that combines evaluation and improvement into a single update sweep using the Bellman Optimality Equation.

---

## 📊 Visualizations & Results

### 1. State-Value Heatmap
The heatmap visualizes the **expected return** from every square. Notice the "gradient of value" that increases as the agent gets closer to the terminal goal at (4,4).



### 2. Optimal Policy (Quiver Plot)
The quiver plot uses vectors (arrows) to show the **Optimal Policy ($\pi^*$)**. These arrows represent the action that maximizes the expected future reward for every state in the grid.



