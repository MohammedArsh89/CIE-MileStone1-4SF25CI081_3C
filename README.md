# NAME:MOHAMMED ARSH
# USN:4SF25CI081
# Netflix Dataset Analysis – Milestone 1

## Overview
This CIE project analyzes a Netflix movies and TV shows dataset using Python, Pandas, and Matplotlib. It demonstrates CSV reading, data understanding, data transformation, null-value handling with mean imputation where applicable, insight generation, and visualization.

## Dataset
- File: `netflix_titles.csv`
- Records: 5,283
- Columns: 11
- Content: Netflix movies and TV shows with release year, runtime, age certification, IMDb score, and vote count.

## Files
- `Netflix_Milestone1_Analysis.ipynb` – complete executable analysis notebook.
- `netflix_titles.csv` – original CSV dataset used for analysis.

## Transformations and null handling
- Dropped the unnecessary row-index column.
- Converted analytical fields to numeric types where appropriate.
- Imputed missing `imdb_votes` values using the column mean.
- Replaced missing descriptions with `Not available`.
- Replaced missing age certifications with `Not Rated` because this is categorical data and mean imputation is not meaningful.
- Added `release_decade` and `runtime_category`.

## Main findings
- 5,283 titles: 3,407 movies and 1,876 TV shows.
- Average IMDb score: TV shows approximately 7.02; movies approximately 6.27.
- `age_certification` contains 2,285 missing values.
- `imdb_votes` contains 16 missing values; mean imputation is used for these numeric nulls.
- `description` contains 5 missing values.
