# Data Description

This directory contains the datasets used to construct and analyze accessibility networks for the London Underground.

## File Overview

### `London_Accessible_Network.csv`
This file contains the accessible network used in the analysis. It represents the subset of stations and connections included in the accessibility network.

### `London_Income_Data.xlsx`
This file contains income-related data used in the analysis. These data are linked to stations through geographic matching.

### `London_Population_Data.csv`
This file contains population-related data used in the analysis. These data are used to provide demographic context for the network.

### `london.connections_named.csv`
This file contains the named connections between stations in the London Underground network. It is used to construct the full network graph.

### `london.stations.csv`
This file contains station-level information for the London Underground network, such as station names and other metadata used in network construction.

## Data Integration

The datasets are combined as follows:

- `london.stations.csv` and `london.connections_named.csv` are used to build the full transit network
- `London_Accessible_Network.csv` defines the accessible subnetwork used in the analysis
- `London_Income_Data.xlsx` and `London_Population_Data.csv` provide contextual socioeconomic and demographic information

## Sources

These datasets are based on publicly available transit and demographic data sources, including Transport for London (TfL) and related public datasets.

## Notes and Limitations

- Accessibility is treated as a static property
- Network edges represent connectivity only and do not include travel time or service frequency
- Income and population data are linked through geographic aggregation and may not align exactly with individual station locations
