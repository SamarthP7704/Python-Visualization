Python Data Visualization with Seaborn
This project is a collection of data visualization examples using the Seaborn and Matplotlib libraries in Python. It explores the California Housing dataset to demonstrate various plotting techniques for statistical analysis.

📋 Table of Contents
Overview

Prerequisites

Dataset

Visualizations Included

Future Improvements

📖 Overview
The purpose of this notebook is to learn and implement different types of statistical plots to understand data distributions and relationships. It uses the California Housing dataset to map variables like population, households, and income.

⚙️ Prerequisites
To run this notebook, you will need the following Python libraries installed:

Pandas: For data manipulation.

Seaborn: For statistical data visualization.

Matplotlib: For underlying plot rendering.

Bash
pip install pandas seaborn matplotlib
📊 Dataset
The project uses the California Housing Test dataset (california_housing_test.csv). Key features used in the analysis include:

population: Total number of people residing in a block.

households: Total number of households.

median_income: Median income for households within a block.

latitude: Geographical coordinate.

total_rooms: Total number of rooms in a block.

📈 Visualizations Included
The notebook covers the following types of plots:

1. Distribution Plots

Distplot (KDE): Visualizes the univariate distribution of the 'Population' column, showing both a histogram and a Kernel Density Estimate (KDE).

Distplot (Rug): A histogram of the population with the KDE turned off, featuring a "rug" plot to show individual data points along the x-axis.

2. Relationship Plots

Joint Plot (Scatter): Compares population vs. households. Displays a scatter plot in the center and histograms on the margins to show individual distributions.

Joint Plot (Hexbin): A variation of the joint plot using hexagonal bins (kind="hex") to visualize data density in areas with many overlapping points.

Pair Plot: A grid of plots comparing relationships between latitude, housing_median_age, and total_rooms simultaneously.

3. Categorical Plots

Box Plot: Used to visualize the distribution of median_income across different population groups (checking for outliers).

Swarm Plot: Visualizes latitude against total_rooms to show the distribution of observations without overlapping points.

Strip Plot: Similar to a swarm plot but adds "jitter" to spread points out, useful for visualizing total_rooms distribution across latitudes.

📝 Notes & Deprecation Warnings
Seaborn Updates: The code currently uses sns.distplot, which is deprecated in newer versions of Seaborn. For future iterations, consider using sns.displot or sns.histplot.

Performance: Swarm plots scale poorly with large datasets. If the code takes a long time to run, consider using a Strip plot or Violin plot instead.
