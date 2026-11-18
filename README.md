# Diurnal Complementarity of Wind Power in California and Wyoming

Energy Meteorology semester project | Xinhao Li

## Project Overview

This project looks at whether wind power from selected plants in California (CA) and Wyoming (WY) can complement each other over a 24-hour cycle. I want to see whether higher output in one state tends to occur when output in the other is lower, and whether this makes their combined output more stable.

My hypothesis is that the two groups of plants reach their daily peaks at different times. I will test whether this timing difference helps smooth their combined output and whether the results change by season.

## Data Source

I plan to use hourly wind power estimates from [PLUSWIND](https://wdh.energy.gov/project/pluswind) for 2018–2021. The dataset provides modeled capacity factors, which show output as a fraction of each plant's rated capacity.

I will start with `ERA5 CF (density and loss adjusted)` and use the `gmt` column to match the same hours in both states. I also plan to repeat the comparison with the corresponding HRRR estimates to see whether the results depend on the model.

### How to Download the Data

1. Sign in to Wind Data Hub and open the [PLUSWIND download page](https://wdh.energy.gov/ds/pluswind/plant.c0).
2. Use the plant list on the project page to find plant IDs in CA and WY.
3. Download the available CSV files for the selected plants and years. For the first test, start with one plant in each state for 2019.
4. Save the files locally in `data/raw/`. I will add the final plant IDs and filenames here after checking the files.

Dataset DOI: [10.21947/1903602](https://doi.org/10.21947/1903602)

## Planned Analysis

1. Match the CA and WY records by UTC timestamp and check for missing hours.
2. Plot the average 24-hour capacity factor cycle for each state by season. This will show when output is usually highest and lowest.
3. Make a scatter plot of CA versus WY capacity factors for matched hours. This will show whether one tends to be high when the other is low.
4. Use a bar chart to compare the variability of the CA, WY, and combined capacity factors. I will weight plants by rated capacity when combining their output.

The results will describe the selected plants. PLUSWIND provides modeled estimates, so I will check whether ERA5 and HRRR lead to similar conclusions.

## Project Status

The first step is to check the available plant files and test the analysis with one plant from each state. I will add the selected plant list and instructions for running the code as the project develops.
