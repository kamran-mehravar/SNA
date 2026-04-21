# SNA

Social Network Analysis project focused on diffusion modeling and simulation using **NDlib**.

## Overview

This repository contains a Social Network Analysis project developed at the **University of Pisa**. The main objective is to simulate and analyze diffusion processes on networks using the **NDlib** Python library.

The project studies several classical diffusion models:

- SI
- SIS
- SIR
- Threshold Model

These models are tested both on:

- **crawled real-world data**
- **synthetic graphs**, including:
  - Erdős–Rényi (ER)
  - VA graphs

The goal is to compare how different diffusion processes behave when changing model parameters and initial conditions. 

## Main Idea

The project focuses on simulating spreading processes over networks and analyzing the results under different experimental conditions.

According to the repository description, the work includes:

- simulation of diffusion models discussed during the course
- experiments on crawled network data
- experiments on synthetic graphs
- analysis of the simulation outcomes by varying:
  - model parameters
  - initial conditions 

## Diffusion Models

The repository README explicitly mentions the following models:

- **SI**
- **SIS**
- **SIR**
- **Threshold Model**

These are standard models used in social network analysis to study how information, behaviors, or contagion spread over a network.

## Repository Structure

The repository currently contains the following main files:

```text
.
├── AI_network_2 _2.ipynb
├── Final_report_group8.pdf
├── Projection.ipynb
├── README.md
└── weighted_net_amsterdam.csv
```

This suggests that the project includes:

- Jupyter notebooks for experimentation and simulation
- a final PDF report
- a dataset related to a weighted Amsterdam network
- a projection step used to estimate graph parameters for synthetic experiments 

## Dataset and Projection

The repository includes a file named:

- `weighted_net_amsterdam.csv`

and a notebook named:

- `Projection.ipynb`

The current project description explains that the projection phase must be run first, and its results must then be used in later parts of the workflow. In particular, the generated values are used in synthetic graph definitions such as:

```python
g = nx.erdos_renyi_graph(11110, 226.9941/11110)
```

The README also notes that these values may vary from one run to another because node and edge selection is random. 
## Experimental Workflow

A typical workflow for this project is:

1. upload the dataset
2. run the projection part
3. collect the projection results
4. use those values to define the synthetic graph
5. run the diffusion simulations
6. compare the results across different models and parameter settings

The repository README explicitly states that the projection results must be collected and then used as input values for the network definition step. 

## Running the Project

According to the repository description, the code should be executed in **Google Colab**, because the simulations require substantial resources.

Recommended environment:

- [Google Colab](https://colab.research.google.com/)

The README explicitly states that Colab should be used as the working environment for running the code. 

## Tech Stack

- Python
- Jupyter Notebook
- NDlib
- NetworkX
- Google Colab

GitHub currently reports the repository language as **100% Jupyter Notebook**. 

## Documentation

The repository includes:

- `Final_report_group8.pdf`

This file likely contains the final report for the project, including methodology, simulations, and results.

## Design Goals

This project was developed with the following goals:

- simulate diffusion processes on networks
- compare spreading models on real and synthetic data
- study the effect of parameters and initial conditions
- use projection-based graph construction
- analyze social network behavior through computational experiments

## Notes

This repository represents a Social Network Analysis project based on diffusion modeling with **NDlib**. It combines projection-based graph setup, synthetic and real network experiments, and simulation analysis using Jupyter notebooks.
## Related Work


It also connects  work on **spectral clustering** in **CDlib**:

- [CDlib Spectral Algorithm Documentation](https://cdlib.readthedocs.io/en/latest/reference/generated/cdlib.algorithms.spectral.html)

## License

This project is licensed under the MIT License.
