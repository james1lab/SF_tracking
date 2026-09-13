This repository provides the global extratropical cyclone (ETC) trajectory dataset produced for the manuscript:

A Sophisticated Lagrangian Tracking Algorithm with Vorticity–Streamfunction and High-Order Spectral Filtering: Application to Global Extratropical Cyclones
Jae-Deok Lee, Eun-Chul Chang, and Ui-Yong Byun

The trajectories were identified by applying a vorticity–streamfunction-based Lagrangian tracking method to ERA5 reanalysis data for 1990–2024.

Dataset

Input dataset: ERA5 reanalysis

Analysis period: 1990–2024

Input resolution: 0.25° and 6 h

Coverage: Northern and Southern Hemispheres

Completed trajectories: 29,342 in the Northern Hemisphere and 28,563 in the Southern Hemisphere

The public data files are provided in the data/ directory. Definitions of the variables, units, and missing-value conventions are provided in docs/DATA_DICTIONARY.md.

Before release: Add the final data filenames and formats here.


Six-hourly Southern Hemisphere ETC trajectories

Method overview

The method uses a rotational streamfunction obtained from spectrally filtered lower-tropospheric relative vorticity. Candidate ETC centers are evaluated at 900, 850, 800, and 750 hPa to identify vertically consistent cyclone-scale circulation and are linked at 6-h intervals to construct trajectories. Only completed trajectories satisfying the detection, screening, and minimum-lifetime criteria described in the manuscript are included in this repository.

For the complete filtering procedure, detection thresholds, trajectory-linking criteria, and sensitivity analyses, please refer to the associated manuscript and Supporting Information.

Code availability

This repository contains the resulting ETC trajectory dataset and its documentation. The source code for the tracking algorithm is not publicly distributed because it is currently being used in ongoing research projects. The code is available from the corresponding author upon reasonable request for research and reproducibility purposes.
