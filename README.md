# UK House Prices vs Bank Rate (2021–2023)

How did house prices across England's nine regions change as the Bank of England raised interest rates from 0.1% to 5%?

## Data
- **UK House Price Index** (HM Land Registry), average prices by region and property type
- **Bank Rate history** (Bank of England)

## Method
- Filtered the House Price Index to the nine English regions (`Area_Code` starting with `E12`)
- Used `pd.merge_asof` to match each month to the Bank Rate in force at the time
- Compared the percentage change in prices between December 2021 and August 2023 by region and property type
- Visualised long-term trends and regional changes with line and bar charts

## Key findings
- Prices still rose almost everywhere despite the rate rises
- The North East grew most (8.6–10.5%), while London grew least, with London flats falling slightly (−0.2%)
- Flats were the weakest property type in every region

## Limitations
- Prices are not adjusted for inflation
- The analysis shows correlation, not causation
- House prices react slowly, so some effects may appear after August 2023

## Tools
Python, pandas, matplotlib, Jupyter Notebook

## How to run
Open `house_price_analysis.ipynb` in Jupyter Notebook with the data files in the same folder.
