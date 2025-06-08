# Aviation Accident Analysis

## Project Overview

This project analyzes aviation accident data to help an airline insurer identify the safest airplane makes and models. The focus is on planes still potentially active (1983 onward), with separate analysis for small (<20 passengers) and large (≥20 passengers) aircraft.

## Dataset

- Source: Kaggle
- Filtered to aircraft from 1983+
- Separate groups: small and large aircraft
- Only models with at least 10 incidents included

## Data Cleaning

Performed in Aviation_Accidents_Cleaning.ipynb:
- Drop columns where more than 50% of rows are missing
- Created new columns:
  - SeriousOrFatal_Rate: share of passengers seriously/fatally injured
  - Aircraft_Destroyed: 1 if destroyed, 0 otherwise
  - Make_Model: combined Make and Model
- Standardized manufacturer names and cleaned categorical variables

## Analysis

Performed in Aviation_Accidents_Data_Analysis.ipynb:

### Small Aircraft Recommendations
- Safest models: SCHWEIZER 269, PZL-SWIDNIK W-3A, HUGHES 369

### Large Aircraft Recommendations
- Safest models: MCDONNELL-DOUGLAS DC-9, AIRBUS A320, BOEING 737

## Key Findings

- Commercial jets show consistent safety
- Poor weather conditions (IMC) and reciprocating engines increase injury/destruction risk

## Repository Structure

- data/
  - AviationData.csv
  - cleaned_aviation_data.csv
- Aviation_Accidents_Cleaning.ipynb
- Aviation_Accidents_Data_Analysis.ipynb
- README.md

## How to Run

1. Clone the repo
2. Run the cleaning notebook
3. Run the analysis notebook

