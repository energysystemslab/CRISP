# CRISP: A framework for comprehensive State of Health (SOH) assessment.

CRISP (Comprehensive Real-time Insights for State-of-health Prediction) is a physics-based software developed in Python for the comprehensive assessment of the SOH of lithium-ion batteries.

LIB Degradation Analysis Code
This repository contains Python code for lithium-ion battery (LIB) degradation analysis. 

Key Features
Imports half-cell potential data for anode and cathode.
Processes specific capacity based on active material mass.
Generates plots for half-cell and full-cell data.
Optimizes parameters for half-cell reconstruction and calculates metrics like N/P ratio, capacity fade, and internal resistance.
Provides visualizations of data.

Usage
Set up the directory paths and datasets as described in the inline comments.
Adjust initial parameters and bounds for different DOD conditions.
Run the script to generate plots and output metrics for analysis.
Dependencies
The following Python libraries are required:
numpy
pandas
scipy
matplotlib
sklearn
scipy.signal.savgol_filter

Output
Half-cell and full-cell voltage profiles and DVA.
Parameter optimization results for each RPT condition (slippages and massess).
Derived metrics such as capacity, percentage capacity, internal resistance and N/P ratio.

Notes
File Structure: Ensure that the dataset is organized as follows:
	Half-cell data files are in half_cell_data subdirectories.
	Full-cell data files are in RPT_* folders.
The optimization parameters may require fine-tuning depending on specific test conditions.
Ensure that data files follow the naming conventions used in the code.
For each DOD condition, adjust the initial_guess and bounds variables as indicated in the comments.
