# US Crime Data Statistical Analysis

**Notebook:** `crime_statistics.ipynb`

## Overview

This project performs a comprehensive statistical analysis of United States crime data, integrating multiple datasets to explore trends in offense rates, victimization, recidivism, and firearm legislation relationships.

## Datasets

The analysis uses data from four primary sources:

1. **National Incident-Based Reporting System (NIBRS):** Offense counts by category and year (`nibrs_offense_count.csv`).
2. **State Population Data:** U.S. state populations from 1991–2021 (`population_states_1991_2021.csv`).
3. **National Crime Victimization Survey (NCVS):** Cleaned personal and property victimization data (`pcvdf_clean.csv` and `ppdf_clean.csv`).
4. **National Institute of Justice (NIJ) Recidivism:** Individuals’ recidivism records, including demographic and offense details (`njidf_clean.csv`).
5. **Firearm Legislation Dataset:** State-level firearm laws (`firearm_laws.csv`).

## Project Structure

The notebook is organized into the following sections:

1. **Data Loading**: Importing and inspecting all datasets.
2. **Exploratory Analysis**:

   * Yearly national offense rates for top five offense categories.
   * State-level offense rates and heatmaps.
   * Trends in personal and property victimization rates.
3. **Recidivism Analysis**:

   * Data cleaning and feature engineering (e.g., ordinal encoding of `age_at_release`).
   * Fitting linear regression models to identify factors influencing recidivism.
4. **Bonus Task**:

   * Building a machine learning pipeline to predict recidivism within three years of release.

## Key Findings

* Identification of the top five most frequent offense categories nationally over time.
* Geographic variation in offense rates across states.
* Insights into demographic and legal factors affecting recidivism.
* Initial predictive performance of a recidivism classification model.

## Requirements

* Python 3.8+
* Jupyter Notebook
* Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

Install dependencies with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Usage

1. Clone the repository or download the notebook.
2. Ensure data files are located in the paths specified in the notebook or update paths accordingly.
3. Launch Jupyter and open `crime_statistics.ipynb`:

   ```bash
   jupyter notebook crime_statistics.ipynb
   ```
4. Run cells sequentially to reproduce the analysis and visualizations.

## Authors
- [Mohamed Ahmed](https://github.com/mahmedken)
- [Khaled El Bastawesy](https://github.com/khaledElbastawisy)

## License

This project is released under the MIT License. See [LICENSE](LICENSE) for details.
