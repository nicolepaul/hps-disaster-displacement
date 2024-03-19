# Household displacement after disasters in the United States

## Overview

In 2022, more than 1.3% of the adult population (3.3M) in the United States was displaced by disasters [(AP News)](https://apnews.com/article/natural-disasters-indiana-florida-climate-and-environment-0bfdab41b233feba55e08382a0594258). This repository includes code to investigate the public use files (PUF) from the [**United States Household Pulse Survey (HPS)**](https://www.census.gov/programs-surveys/household-pulse-survey.html). Information regarding displacement following disasters was introduced from Phase 3.7 (Week 52). The availability of microdata allows an exploration of various factors that may be associated longer displacement durations.

## Contents

This repository contains Python code to perform exploratory analysis and fit machine learning models to the HPS data. This work is being submitted for publication.

This code mainly comprises four Jupyter Notebooks:

- [**0. Exploratory analysis.ipynb**](/0. Exploratory analysis.ipynb): Basic data analysis to get descriptive statistics and explore trends between factors related to household displacement and return after disasters
- [**1. Classification tree.ipynb**](/1. Classification tree.ipynb): Fits a decision tree model for household displacement durations
- [**2. Random forest.ipynb**](/2. Random forest.ipynb): Fits a random forest model for household displacement durations
- [**3. Model variant - physical factors only.ipynb**](/3. Model variant - physical factors only.ipynb): Fits a decision tree model, but only considers physical factors typically included within disaster risk analyses

Most of the notebooks only take a few minutes to run. However, the random forest model takes several hours to fit. Therefore, the best-fit random forest model from the previous analysis is saved as `best_rf.sav` and can be loaded directly.