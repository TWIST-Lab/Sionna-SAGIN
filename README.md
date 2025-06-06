# Sionna-SAGIN
This repository contains a simulation and evaluation framework for a UAV-assisted Space-Air-Ground Integrated Network (SAGIN) architecture designed to improve Direct-to-Cell (D2C) communication performance in diverse terrains. The code leverages realistic propagation and fading models to simulate signal quality, throughput, latency, and error rates for baseline and UAV-relayed architectures.

## Introduction 
Traditional D2C communication suffers from high propagation losses, capacity bottlenecks, and limited reliability in remote or disaster-stricken areas. This framework evaluates a SAGIN-based solution where UAVs serve as adaptive relays between LEO satellites and user terminals (UTs), decoupling ionospheric and multipath effects. We consider three communication topologies:  
- **Trad-D2C**: direct satellite-to-UT links  
- **SAGIN-D2C**: relayed via UAVs at fixed positions  
- **Opt-SAGIN-D2C**: relayed via UAVs with optimized 3D placement  

Realistic terrain-aware shadowing and fading models are used across Desert, Mountain, and City environments.

## Setup and Requirements
- Python 3.8+
- Jupyter Notebook
- Required packages:  
  `tensorflow`, `sionna`, `optuna`, `numpy`, `scipy`, `matplotlib`, `seaborn`, `pandas`

## Usage

Launch Jupyter and open the evaluation_notebook.ipynb.

Execute all cells to simulate performance over various terrains and topologies.

The notebook outputs:

CSV file with SNR, BLER, latency, and throughput results

Plots for comparative analysis in results/ and plots/ directories

## Citation
This work was submitted to MILCOM 2025:

Abdullah Al Noman, Talip Tolga Sarı, Sunday Amatare, Gokhan Secinti, and Debashri Roy,
"Space-Air-Ground Network for Direct-to-Cell Communication,"
IEEE Military Communications Conference (MILCOM), October 2025 [Submitted].
