# Peer Town Business Gaps
## Overview
This project is an open, reproducible Python analysis that compares cities to structurally similar peer towns to identify differences in local business ecosystems.

Rather than asking “what businesses should exist here,” the project asks a narrower, more defensible question:  

> What kinds of business categories and brands tend to appear in towns with similar size, demographics, and regional roles and which of those are absent locally?  

The goal is decision support, not recommendations.

## Status
** Active development. **

Notebooks and results are exploratory and subject to change.

This repository demonstrates methodology, not conclusions or endorsements.

## Motivation
Small and mid-sized cities often compare themselves to larger metros or aspirational examples that are not structurally comparable. This project takes a different approach by:

• Identifying peer towns based on measurable characteristics  
• Comparing business presence across those peers  
• Surfacing patterns that are common elsewhere but missing locally  

The initial case study focuses on Kerrville, Texas, but the framework is designed to be reusable for other cities.
## Approach (High-Level)
• Define candidate towns using population and geographic filters  
• Identify peer towns using demographic and economic similarity (nearest neighbors)  
• Collect business location data from OpenStreetMap  
• Normalize and categorize businesses by type and brand  
• Compare frequency across peer towns to identify gaps  
• Test sensitivity to peer definitions and assumptions  

County-level data is used for context (for example, county seat status), while the city is the primary unit of analysis.
## Data Sources
This project uses publicly available data only:

• U.S. Census Bureau (ACS 5-Year Estimates)  
• Population, income, age, education, and related demographics  
• TIGER/Line Shapefiles  
• City boundaries and geographic relationships  
• OpenStreetMap (via Overpass / OSMnx)  
• Business and amenity points of interest  

No proprietary datasets are required.
## What This Project Is Not
• Not a list of “businesses the city should recruit”  
• Not a measure of business quality or success  
• Not a ranking of cities  
• Not an economic development plan  

Local factors such as zoning, workforce availability, seasonality, tourism, and existing competition matter and are not fully captured by the data.
## Repository Structure
/notebooks      Jupyter notebooks (numbered, sequential)
/src            Reusable Python functions
/data
  /raw          Source data pulls
  /processed    Cleaned and derived datasets
/outputs        Tables and figures for reporting

## Reuse
The analysis is designed to be adaptable:
• Change the target city  
• Adjust peer selection criteria  
• Focus on categories instead of brands  
• Limit scope to specific business types (food, health, services, etc.)  

All assumptions are documented in code and notebooks.
## License
** MIT License. **  

Feel free to reuse, adapt, and extend with attribution.

## Contact / Notes
This repository is maintained as a civic analysis and learning project.  

Feedback, corrections, and suggestions are welcome.
