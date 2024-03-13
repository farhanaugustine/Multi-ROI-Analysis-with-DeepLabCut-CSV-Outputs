# Multiple ROI Analysis with DeepLabCut CSV Files

## Overview
This project involves analyzing multiple Regions of Interest (ROIs) using CSV files generated by DeepLabCut, a machine-learning tool for animal pose estimation.

![Screenshot 2024-03-13 092658](https://github.com/farhanaugustine/Multi-ROI-Analysis-with-DeepLabCut-CSV-Outputs/assets/54376988/5c2b5d5e-d7c1-410d-9862-6d85a158d1fa)



## Features
- **Import Libraries**: Utilizes essential Python libraries for data manipulation and visualization.
- **Data Import**: Loads CSV data for analysis, focusing on body part coordinates and likelihoods.
- **Body Part Data**: Creates a dictionary mapping body parts to their respective coordinates and likelihood values.
- **ROI Drawing**: Allows users to draw ROIs and calculates the time spent by subjects within these regions.
- **Temporal Analysis**: Analyzes the number of entries and exits from ROIs, including the first entry and the sequence of visits.
- **Velocity Calculation**: Computes velocities for each body part and graphs them per ROI.
- **Graphing**: Visualizes data such as the number of entries and exits per ROI and the average velocities.

## Usage
To use this project, follow the steps outlined in the code cells, from importing libraries to graphing the results. Customize the ROI names, colors, and body parts as per your experimental setup.

## Data Structure
The data is structured with body part coordinates and likelihoods, which are used to calculate distances, velocities, and time spent in ROIs. In addition, the code allows for the tracking of sequences and frequency of ROI visits.

## Visualization
The project comprises features that allow the plotting of data and ROIs, thus providing valuable insights into the animal's movements and behavior patterns over time. Please note that certain blocks of code use a paired-body part system and have constraints on the minimum number of frames that the animal must be present inside/outside the ROI before entry/exit can be counted.

## Customization
Users can modify the body parts, ROIs, and other parameters (e.g., `debounce_frames` and `body_part_pairs`) to fit their research needs.
