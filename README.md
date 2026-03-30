# expressway-risk-analysis
Southern Expressway Road Risk Analysis using GIS
Project Overview

This project presents a GIS-based road risk analysis for a section of the Southern Expressway (E01), Sri Lanka, using International Roughness Index (IRI) and road curvature data. The objective of this study is to identify high-risk road segments (accident hotspots) using spatial analysis and linear referencing techniques in QGIS.

This project combines Transportation Engineering, GIS, and Data Analysis to develop a road risk model and visualize risk zones along the expressway.

Study Area

The study area covers the Gelanigama to Pinnaduwa section of the Southern Expressway, approximately 32.1 km in length.

Objectives
Generate points along the expressway at 100 m intervals
Calculate chainage for each point
Assign IRI values using linear referencing
Calculate road curvature
Develop a Risk Index model
Classify risk levels using Natural Breaks (Jenks)
Identify accident hotspot locations
Calculate length and percentage of high-risk road segments
Methodology

The GIS workflow used in this project is shown below:

Extract expressway centerline
Generate points every 100 m
Calculate chainage (km)
Assign IRI values using linear referencing
Calculate curvature
Calculate Risk Index
Classify risk using Jenks Natural Breaks
Identify accident hotspots
Buffer analysis
Clip road by risk zones
Dissolve road segments
Calculate road length
Calculate risk percentage
Risk Model

The Risk Index was calculated using the following weighted model:

𝑅
𝑖
𝑠
𝑘
=
0.6
×
𝐼
𝑅
𝐼
+
0.4
×
𝐶
𝑢
𝑟
𝑣
𝑎
𝑡
𝑢
𝑟
𝑒
Risk=0.6×IRI+0.4×Curvature

Where:

IRI = International Roughness Index (road roughness)
Curvature = Road curvature (deflection angle)
IRI was given higher weight because road surface condition has a greater influence on vehicle control and accident probability.
Risk Classification

Risk values were classified into three categories:

Risk Value	Risk Level
R < 40	Low Risk
40 ≤ R < 70	Moderate Risk
R ≥ 70	High Risk

High-risk segments were identified as accident hotspots.

Results
Risk Level	Length (km)	Percentage
High Risk	6.7 km	20.9%
Moderate Risk	11.2 km	30.5%
Low Risk	14.2 km	44.3%
Total	32.1 km	100%

The results show that approximately 20.9% of the road segment falls into the high-risk category, indicating sections that require maintenance and safety improvements.

Tools & Technologies Used
QGIS
Microsoft Excel
GIS Spatial Analysis
Linear Referencing
HTML, CSS, JavaScript
GitHub Pages
Project Website

You can view the project website here:

https://yourusername.github.io/expressway-risk-analysis/
Conclusion

This study demonstrates how GIS and spatial analysis can be used to identify accident-prone road segments using road condition and geometric data. The developed risk model can support road authorities in decision-making related to road maintenance, safety improvements, and accident prevention.

Author

Sithum Yapa
Undergraduate – Engineering / Data Science / GIS
Sri Lanka

License

This project is for academic and research purposes.
