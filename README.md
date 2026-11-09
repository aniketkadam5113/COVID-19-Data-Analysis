# COVID-19 Data Analysis

## Project Overview

This project explores the global impact of COVID-19 using confirmed cases, deaths, and recoveries data. The analysis uses Python and its data analysis libraries to clean, transform, merge, analyze, and visualize COVID-19 data.

The objective is to identify pandemic trends, compare country-level statistics, and derive meaningful insights through exploratory data analysis.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- Microsoft Excel

## Dataset

The project uses an Excel dataset containing three worksheets:

- COVID-19 Confirmed Cases
- COVID-19 Deaths
- COVID-19 Recoveries

**Analysis period:** January 22, 2020 – May 29, 2021.

## Project Workflow

### 1. Data Loading and Exploration
- Imported datasets using Pandas.
- Explored dataset dimensions, columns, and data types.
- Examined country and date information.

### 2. Data Cleaning
- Identified missing values.
- Handled missing daily values using forward filling.
- Replaced missing Province/State values with "All Provinces".
- Preserved missing geographical coordinates where appropriate.

### 3. Data Analysis and Visualization
- Analyzed COVID-19 trends across countries.
- Compared confirmed cases over time.
- Visualized China's confirmed cases.
- Identified peak daily new cases in Germany, France, and Italy.
- Compared recovery rates between Canada and Australia.
- Analyzed death rates across Canadian provinces and territories.

### 4. Data Transformation
- Converted the deaths dataset from wide format to long format using Pandas `melt()`.
- Converted date columns into datetime format.
- Calculated country-wise cumulative deaths.
- Identified countries with the highest average daily deaths.
- Visualized cumulative deaths in the United States.

### 5. Data Merging
- Transformed confirmed, deaths, and recovered datasets into long format.
- Aggregated records by country and date.
- Merged the three datasets using Country/Region and Date.
- Analyzed monthly sums for confirmed cases, deaths, and recoveries.

### 6. Combined Data Analysis
- Identified countries with the highest average death rates during 2020.
- Compared recoveries and deaths in South Africa.
- Analyzed monthly recovery ratios for the United States.

## Key Findings

- The United States recorded the highest cumulative deaths in the dataset as of May 29, 2021.
- France experienced the highest single-day surge among Germany, France, and Italy, with 117,900 reported new cases on April 11, 2021.
- Canada had a higher recovery rate than Australia as of December 31, 2020.
- Quebec recorded the highest death rate among Canadian provinces and territories.
- Yemen recorded the highest average daily death-rate percentage among the countries analyzed during 2020.
- South Africa recorded substantially more recoveries than deaths.
- The United States recorded its highest monthly recovery ratio in October 2020.

## Important Data Limitations

- The dataset covers January 22, 2020, to May 29, 2021.
- Some countries have missing or incomplete recovery records.
- US recovery values are zero from January 2021 onwards in the source dataset.
- Monthly sums calculated from cumulative daily figures represent sums of cumulative observations, not actual new monthly cases or deaths.
- Reported statistics may be affected by differences in testing and reporting practices.

## How to Run the Project

1. Clone or download this repository.
2. Install the required Python libraries.
3. Open Jupyter Notebook.
4. Open `COVID_19_Case_Study.ipynb`.
5. Ensure the Excel dataset is available in the expected `dataset/` directory.
6. Execute the notebook cells sequentially.

Install dependencies using:

```bash
pip install -r requirements.txt
```

## Project Structure

```text
COVID-19-Data-Analysis/
│
├── dataset/
│   └── covid_19_dataset.xlsx
│
├── images/
│   └── charts and visualizations
│
├── notebooks/COVID_19_Case_Study.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Conclusion

This project demonstrates practical data analysis skills using Python, Pandas, NumPy, and Matplotlib. It covers data cleaning, exploratory data analysis, data transformation, merging, statistical calculations, and data visualization to understand the global impact of COVID-19.