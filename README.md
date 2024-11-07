
# Quantum Portfolio Optimization

This project implements a quantum portfolio optimization algorithm using Qiskit, inspired by the [Qiskit Finance portfolio optimization tutorial](https://qiskit-community.github.io/qiskit-finance/tutorials/01_portfolio_optimization.html). Quantum portfolio optimization seeks to identify the optimal allocation of assets to maximize returns while minimizing risk, leveraging quantum computing's capabilities for complex optimization problems.

## Overview

Portfolio optimization involves selecting a subset of assets that balances expected returns and risk. By using quantum algorithms like the Quantum Approximate Optimization Algorithm (QAOA) and the Sampling Variational Quantum Eigensolver (SamplingVQE), this project demonstrates a quantum-inspired approach to portfolio optimization within a mean-variance framework.

## Implementation Details

This project builds on Qiskit’s portfolio optimization framework to implement quantum-inspired solutions, including:

- **Quantum Circuit Design**: Tailored quantum circuits for portfolio optimization.
- **Variational Algorithms**: Leveraging QAOA and SamplingVQE for optimal asset selection.
- **Classical Comparison**: Classical optimization methods, such as the NumPy Minimum EigenSolver, for benchmarking.

### Key Parameters

- **Risk Factor (q)**: Controls the level of acceptable risk.
- **Budget (B)**: Number of assets to select.
- **Expected Returns (μ)** and **Covariance Matrix (Σ)**: Define the asset returns and inter-asset correlations.

## Data Source

This project utilizes historical data from a group of 30 backtested trading algorithms for the forex market. The algorithms were analyzed using tick data from **Tick Data Suite**, which provides high-quality data for constructing accurate expected returns and covariance matrices. This is integral to setting up the mean-variance optimization framework for this project.

## Getting Started

### Prerequisites

To run this project locally, ensure the following are installed:
- Python 3.8+
- Jupyter Notebook
- Qiskit and Qiskit Finance

Install the necessary packages via:
```bash
pip install qiskit qiskit-finance jupyter
```

### Running the Project

1. Open the Jupyter Notebook.
2. Follow the steps to initialize the data, set parameters, and run the optimization.
3. Experiment with different quantum backends or simulators to evaluate performance.

## License

This project is licensed under the **Apache License 2.0**. See the [LICENSE](LICENSE.txt) file for more details.
