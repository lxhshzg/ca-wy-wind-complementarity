# Project Checklist

This project asks whether wind power from selected plants in California and Wyoming is more stable when combined and whether the relationship changes by season.

## First GitHub Check

- [x] Add the project question and the PLUSWIND data link to the README.
- [x] Prepare a [starter notebook](01_hourly_comparison.ipynb) to match hourly records and make a first comparison.
- [ ] Check that the README and notebook open on GitHub.
- [ ] Submit the repository URL on Canvas.

## Next Steps for the Analysis

1. **Test with two plants.** Download one 2019 PLUSWIND CSV from each state. Record the plant names, IDs, and original filenames. Follow the instructions in the notebook and turn off demo mode.
2. **Expand the sample.** Check which selected plants have usable matching hours from 2018–2021. Record data gaps and collect rated plant capacities for the combined series.
3. **Compare seasons.** Make a line plot of the average daily cycles, a scatter plot of paired hourly output, and a bar chart comparing hourly variability for CA, WY, and their combined capacity factor.
4. **Check model sensitivity.** Repeat the comparison with HRRR and see whether the main patterns are similar to ERA5.
5. **Report the findings.** Explain whether the selected plants' outputs tend to offset each other, when the combination is smoother, and what the modeled data can tell us.

## How to Try the Notebook

Open `01_hourly_comparison.ipynb` in Jupyter or Colab and run the cells from top to bottom. It uses pandas, NumPy, and matplotlib. For a local Python setup, install them with `python -m pip install pandas numpy matplotlib`.

The demo uses made-up data so the notebook can run before the files are downloaded. Use real PLUSWIND files to report project results. Keep the original CSVs locally in `data/raw/`.
