# ca-wy-wind-complementarity
Energy Meteorology class project on hourly wind power in California and Wyoming.
Diurnal Complementarity of Wind Power in California and Wyoming

Project Overview

This project looks at whether wind power from selected plants in California (CA) and Wyoming (WY) can complement each other throughout the day. I want to see whether higher output in one state tends to occur when output in the other is lower, and whether combining their output makes it more stable. I will also compare these patterns across seasons.

Data Source

I plan to use hourly modeled wind power data from PLUSWIND for 2018–2021. I will start with the ERA5 capacity factor estimates and use the gmt column to match the same hours in both states. Capacity factor shows how much power a plant produces as a fraction of its rated capacity.

How to Download the Data

Open the PLUSWIND download page and sign in to Wind Data Hub.

Use the plant list on the project page to identify wind plants in California and Wyoming.

Download the available CSV files for the selected plants and years. Start with one plant in each state for 2019 to test the analysis.

Save the CSV files in a local data/raw/ folder. I will add the final plant names and IDs after checking data availability.

Dataset DOI: 10.21947/1903602
