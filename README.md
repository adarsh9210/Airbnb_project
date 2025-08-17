# Airbnb EDA Project

This project performs Exploratory Data Analysis (EDA) on Airbnb listing data. The analysis is conducted using Python libraries such as pandas, numpy, matplotlib, and seaborn.

## Project Structure
- `EDA.ipynb`: Jupyter notebook containing all the EDA steps, code, and visualizations.
- `airbnb_raw_data.csv`: The raw Airbnb dataset used for analysis.

## Steps Performed

### 1. Importing Libraries
- numpy
- pandas
- matplotlib
- seaborn

### 2. Data Loading
- The dataset is loaded from `airbnb_raw_data.csv` into a pandas DataFrame.

### 3. Data Inspection
- Displayed columns and checked for missing values.
- Used `df.info()` and `df.describe()` for data overview and statistics.

### 4. Handling Missing Values
- Converted the `last review` column to datetime.
- Filled missing values in `reviews per month` with 0 and in `last review` with the minimum date.
- Dropped rows with missing `NAME` or `host name`.
- Dropped unnecessary columns like `license` and `house_rules`.

### 5. Data Cleaning
- Removed dollar signs from `price` and `service fee` columns and converted them to float.
- Removed duplicate rows.

### 6. Data Visualization
- Distribution of listing prices using histograms.
- Room type distribution using count plots.
- Number of listings by neighbourhood group.
- Boxplot of price vs. room type.

## How to Run
1. Open `EDA.ipynb` in Jupyter Notebook or VS Code.
2. Run the cells sequentially to reproduce the analysis and visualizations.

## Requirements
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn

Install requirements using:
```
pip install pandas numpy matplotlib seaborn
```

## License
This project is for educational purposes only.
