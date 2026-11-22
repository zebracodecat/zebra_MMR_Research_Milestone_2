# Geographic Variation in Maternal Mortality in the United States: Examining Racial Disparities and State-Level Social Factors

A state-level analysis of maternal mortality in the United States from 2020–2024, examining geographic variation, racial disparities, Black population proportions, structural racism, and educational attainment.

**Author:** Erika Agala  
**Course:** CHIP 705, Milestone 02

## Research question

How does maternal mortality vary across U.S. states, and what relationships exist between maternal mortality, Black population proportions, structural racism, and educational attainment?

The project addresses four specific questions:

1. How does maternal mortality vary across U.S. states?
2. Which states have the highest Black maternal mortality rates?
3. Is the proportion of Black residents within a state associated with maternal mortality rates?
4. Is educational attainment associated with Black maternal mortality rates?

## Why this project

Maternal mortality remains an important public health concern in the United States, particularly because of persistent racial and geographic disparities. Black women experience disproportionately high maternal mortality rates compared with other racial and ethnic groups.

Understanding differences across states and examining potential relationships with demographic and social factors can help identify areas for further research and public health intervention.

This project uses publicly available data to explore these patterns and highlight the importance of equitable maternal healthcare, patient advocacy, and improved maternal health outcomes.

## Approach

The analysis follows these steps:

1. Collect state-level overall maternal mortality data for 2020–2024.
2. Obtain Black maternal mortality data for 2020–2024.
3. Collect state population estimates and calculate the proportion of each state's population identified as Black or African American.
4. Incorporate a published state-level structural racism score.
5. Obtain educational attainment data for births to non-Hispanic Black mothers from 2022–2024.
6. Clean and combine the datasets using state names.
7. Examine descriptive statistics and missing data.
8. Create geographic maps showing overall maternal mortality, Black maternal mortality, Black population proportions, and educational attainment.
9. Calculate Pearson correlations to examine relationships among the study variables.
10. Perform multiple linear regression analyses for overall and Black maternal mortality, and a simple linear regression examining educational attainment and Black maternal mortality.

Analyses use available observations for each variable and statistical model. Therefore, sample sizes vary depending on data availability.

## Files in this repository

- `STATE_MMR_COMB_DATA.csv` — combined state-level dataset used for the analysis.
- `.ipynb` notebook file — the Jupyter notebook containing the data cleaning, analysis, visualizations, and statistical models.
- `README.md` — this file, describing the project and how to run the notebook.

## Data sources

The project uses publicly available data from the following sources:

- Congressional Research Service: State-level overall maternal mortality data, 2020–2024.
- America's Health Rankings: Black maternal mortality data, 2020–2024.
- CDC WONDER: Single-Race Population Estimates, 2020–2024.
- Siegel and colleagues: Published state-level structural racism measure.
- CDC WONDER: Natality Expanded database, 2022–2024.
- U.S. Census Bureau: 2024 TIGER/Line state geographic boundaries.

Full citations and source links are provided in the research report.

## Variables examined

| Variable | Description |
|---|---|
| `STATE_MMR` | Overall state maternal mortality rate |
| `BLACK_MMR` | Black maternal mortality rate |
| `BLACK_POP` | Proportion of the state population identified as Black |
| `STRUCT_RACISM_SCORE` | Standardized state-level structural racism score |
| `BLACK_BA_PLUS_PCT` | Percentage of births to non-Hispanic Black mothers with a bachelor's degree or higher |

Maternal mortality rates are expressed as deaths per 100,000 live births. Black population proportion is used as a demographic measure, not as the denominator for maternal mortality rates.

## How to run the notebook

The analysis was developed using Python and Jupyter Notebook.

1. Download or clone this GitHub repository.
2. Open the project folder in Visual Studio Code.
3. Open the Jupyter notebook (`.ipynb` file).
4. Make sure the required Python libraries are installed.
5. Confirm that `STATE_MMR_COMB_DATA.csv` is in the same project folder as the notebook.
6. Select the appropriate Python environment or Jupyter kernel.
7. Select **Restart Kernel and Run All** to execute the notebook from beginning to end.

## Python libraries

The analysis uses the following Python libraries:

- pandas
- numpy
- matplotlib
- geopandas
- statsmodels

## Key findings

- Overall maternal mortality rates varied across states, ranging from 10.8 to 41.8 deaths per 100,000 live births.
- Black maternal mortality rates ranged from 31.3 to 106.7 deaths per 100,000 live births among the 27 states with available data.
- The overall maternal mortality regression model was statistically significant.
- Black population proportion was positively associated with overall maternal mortality.
- The Black maternal mortality regression model did not identify statistically significant associations with the selected predictors.
- Educational attainment was not significantly associated with Black maternal mortality in the simple regression model.

## Limitations

This study used state-level observational data and cannot establish individual-level relationships or causation. Data availability varied across states, particularly for Black maternal mortality. The education measure covered 2022–2024, while most maternal mortality measures covered 2020–2024. The findings should be interpreted with these limitations in mind.

## Project goal

The goal of this project is to examine geographic and racial disparities in maternal mortality and identify opportunities for further research, improved patient advocacy, equitable healthcare, and public health intervention.
