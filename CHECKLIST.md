# Project Checklist

This project asks whether selected wind plants in California and Wyoming have different daily patterns and whether combining their output reduces variability.

## GitHub Check

- [x] Add the research question and PLUSWIND download link to the README.
- [x] Prepare the [six-plant notebook](01_hourly_comparison.ipynb) and run it with the six 2019 PLUSWIND files.
- [ ] Update the files in the GitHub repository and check that the notebook opens.
- [ ] Submit the repository URL on Canvas.

## Running the Notebook

Open `01_hourly_comparison.ipynb` in Google Colab. Choose **Runtime → Run all** and select all six CSVs at the upload prompt. The first section of the notebook lists their plant IDs. Keep the filenames from PLUSWIND.

For local Jupyter, put the files in `data/raw/`. The notebook uses pandas, NumPy, and matplotlib. Keep the original CSVs locally and use the official link in the README for access.

## Next Steps

1. Check which of the six plants have complete matching hours in 2018, 2020, and 2021.
2. Compare the 24-hour patterns across seasons and check if the results repeat across years.
3. Repeat the analysis with the HRRR estimates. Compare equal-weight results with an average weighted by rated plant capacity.
4. Add the final figures and explain how much the selected plants complement each other.
