# EEG Signal Connectivity Analysis 

## Overview
This repository contains the analysis of functional connectivity in EEG signals recorded from Patient S001. The project utilizes Phase Locking Value (PLV) and Phase Lag Index (PLI) metrics to study brain region interactions across six different EEG signals, recorded during a resting-state condition. The analysis focuses on understanding how these metrics reveal insights into the connectivity strength and directionality between various brain regions. **The EEG data used in this analysis was collected from Physionet**.

## Objectives
The goal of this project is to investigate functional connectivity using EEG signals and to provide insights into how different regions of the brain interact in a resting-state condition. The report includes visualizations such as heatmaps and bar plots to represent connectivity strengths, and it discusses the implications of the findings.

## Methodology
1. **EEG Signals**: Six signals from Patient S001 were analyzed, each containing 64 EEG channels.
2. **Segmentation**: Each signal was segmented into overlapping windows with the following parameters:
   - Sampling frequency: 160 Hz
   - Window duration: 2 seconds (320 samples)
   - Window shift: 0.5 seconds (80 samples)
3. **Metrics Computed**:
   - **PLV (Phase Locking Value)**: Used to measure synchronization strength between signals.
   - **PLI (Phase Lag Index)**: Used to assess directional connectivity, excluding spurious synchronizations.

## Results
The analysis reveals insights into the functional connectivity of the brain:
- **Heatmaps**: Visualizations of PLV and PLI for Signal 4 were generated to analyze pairwise channel connectivity.
- **Bar Plots**: The average PLV and PLI per channel were calculated and displayed for Signal 4.
- **Top Connected Channels**: A list of the top 10 most connected EEG channels based on both PLV and PLI.

### Example Results for Signal 4:
- **PLV Heatmap**: Shows regions of high synchronization.
- **PLI Heatmap**: Displays directional connectivity between channels.

## Code and Execution

### Requirements:
- Python 3.x
- NumPy
- SciPy
- Matplotlib
- Pandas
- MNE (for EEG processing)

### Data Source
The EEG data used for this analysis was obtained from [Physionet](https://physionet.org), a platform offering accessible biomedical datasets.
