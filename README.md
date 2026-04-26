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

# Summary:
This work evaluates neuromorphic (Loihi 2) versus GPU execution for time-series forecasting tasks, focusing on:
- Energy efficiency
- Accuracy tradeoffs
- Architectural differences between SNNs and ANNs
- Cross-dataset generalization

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

## Note:
The requirements file does not install Intel Loihi SDKs. Loihi software must be installed separately through Intel’s NxSDK or Lava installation process, which requires access approval. See  **Intel_INRC_on_LAVA_FAQs.pdf**. 

## Getting Started:
```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>  # Use Terminal/Command Prompt
```
RingSNN Implementations: 
Will require installation of Lava for Loihi Implementation. 
For more Instructions on Installing Intel Loihi including transferring files from the Local Machine to INRC server please see **Intel_INRC_on_LAVA_FAQs.pdf**. 
ANN Implementations: 
As they utilize Nvidia-SMI GPU's Google Colab or an equivalent Interactive Computing Environment would be needed that is capable of handling Nvidia-SMI GPU's. 
**For Google Colab users (Recommended): Make sure you have an active google account and that the files are mounted into your Google Drive prior to executing. Change runtime type to T4 GPU to activate Nvidia-SMI GPU.** 
**For Other Interactive Computing Environment Users: Ensure that Nvidia SMI GPU's are available and are installed in your Interactive Computing Environment. Please delete any instances of Google Colab in the code prior to execution.**


License:
MIT License.
