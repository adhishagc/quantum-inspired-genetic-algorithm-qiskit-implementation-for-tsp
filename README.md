# Implementation of Modified Talbi's Quantum Inspired Genetic Algorithm for Travelling Salesman Problem on an IBM Quantum Computer
---
[![Quantum Computing](https://img.shields.io/badge/Quantum-Qiskit-purple.svg)](https://qiskit.org/)
[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![Publication](https://img.shields.io/badge/Published-Springer-orange.svg)](https://link.springer.com/chapter/10.1007/978-3-030-63089-8_6)

## 📌 Research Overview
This repository contains the groundbreaking implementation of a **Modified Talbi's Quantum-Inspired Genetic Algorithm (QIGA)** designed to solve the **Travelling Salesman Problem (TSP)**. This project marks a significant milestone as it represents the first time Talbi's QIGA has been successfully implemented and executed on a real **IBM Quantum Computer**.

The research associated with this implementation was published in the *Proceedings of the Future Technologies Conference (FTC) 2020*, Volume 2, and is included in the *Advances in Intelligent Systems and Computing* book series (Springer, 2021).

**Reference Paper:**  
[Implementation of Modified Talbi's Quantum Inspired Genetic Algorithm for Travelling Salesman Problem on an IBM Quantum Computer](https://link.springer.com/chapter/10.1007/978-3-030-63089-8_6)  
*Authors: Adhisha Chamikara Gammanpila, T.G.I. Fernando*

---

## 🔬 Methodology and Quantum Innovations

### The Design Limitation in Existing QIGAs
Classical Quantum-Inspired Genetic Algorithms often rely on the assumption that a qubit's state can be duplicated or copied mid-computation to evaluate fitness. However, this fundamental assumption violates the **No-Cloning Theorem** of quantum mechanics, which states that it is impossible to create an identical copy of an arbitrary unknown quantum state without causing it to collapse. As a result, many existing QIGAs are inherently suited only for simulation on classical computers and cannot be deployed on actual quantum hardware.

### The Modified Approach
To overcome this critical blocker, this research introduces a modified version of the algorithm that avoids violating the no-cloning theorem. The state evaluation and fitness calculations are structured such that the algorithm can run natively on quantum circuits. 

The implementation was rigorously tested on two platforms:
1. **IBM Quantum Simulator (Qiskit Aer)**
2. **Real IBM Quantum Computer (IBQ)**

---

## 📊 Results and Convergence

Both the original (simulated) and the modified algorithms demonstrated stability during execution. Below is a comparative analysis of the probability distributions of the qubit states measured on the IBM Simulator versus the real IBM 2-Qubit Quantum Computer.

![IBM Simulator vs IBM Quantum Computer Probabilities](./visuals/simulator_vs_quantum_computer_probabilities.png)
*Figure: Comparative probability measurements demonstrating the algorithm's stability across simulated and real quantum hardware.*

While the study noted that the QIGA did not achieve an optimal level of convergence when compared head-to-head with a highly optimized Classical Genetic Algorithm for the TSP, the primary achievement of this work is the **successful structural modification** that enables complex quantum-inspired evolutionary algorithms to be executed on physical quantum processors.

---

## 💻 Repository Structure & Usage

The project is built using Python and the IBM Qiskit framework. 

*   `quantum_inspired_genetic_algorithm_qiskit_implementation_for_tsp.ipynb`: Main implementation notebook showcasing the quantum circuits, statevectors, and GHZ state preparations.
*   `project_01_python_simulation.ipynb`: Phase 1 of the simulation experiments.
*   `project_01_and_02_python_simulation.ipynb`: Comprehensive simulation comparing classical probabilities with quantum executions.
*   `visuals/`: Contains extracted plots and visualizations from the experiments.

### Prerequisites
To run the notebooks, you will need the IBM Qiskit library:
```bash
pip install qiskit numpy matplotlib
```

*Note: Executing jobs on real IBM Quantum hardware requires an IBM Quantum Experience account and an active API token.*

---
*Pioneering the intersection of Evolutionary Computation and Quantum Mechanics.*
