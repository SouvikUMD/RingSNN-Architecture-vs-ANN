# RingSNN Architecture vs ANN

This repository contains code, experiments, and documentation for the paper:

Energy–Accuracy Tradeoffs in Spiking Neural Networks: Benchmarking Loihi 2 vs GPU using RingSNN and ANN Baselines for Time-Series Regression Forecasting.

The project includes:
- RingSNN architecture implementations
- ANN baselines including CNN, CNN-LSTM, LSTM, and GRU
- Energy and accuracy benchmarking scripts
- Experimental results and plots

# Intel Loihi Requirement:
The RingSNN implementation in this repository is designed for execution on Intel Loihi neuromorphic hardware. Running the full RingSNN pipeline requires access to Loihi 1 or Loihi 2 hardware and the associated Intel NxSDK or Lava framework. CPU-only execution is supported for ANN baselines but not for the neuromorphic RingSNN backend.

# Repository Contents:
- ANN Comparison
  Implementations of ANN baselines used in the study.

- RingSNN
  Core RingSNN architecture and training pipeline.

- RingSNN_Gated+Residual
  Extended RingSNN variants with gating and residual connections.

- Energy-Accuracy Tradeoff Plots
  Visualizations and analysis notebooks.

- Paper PDFs
  Final submission and supplementary materials.

# Installation:
If you plan to run the ANN baselines or preprocessing scripts, install the Python dependencies using:
pip install -r requirements.txt

## Note:
The requirements file does not install Intel Loihi SDKs. Loihi software must be installed separately through Intel’s NxSDK or Lava installation process, which requires access approval.

## Getting Started:
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
pip install -r requirements.txt

# Summary:
This work evaluates neuromorphic (Loihi 2) versus GPU execution for time-series forecasting tasks, focusing on:
- Energy efficiency
- Accuracy tradeoffs
- Architectural differences between SNNs and ANNs
- Cross-dataset generalization

License:
MIT License.
