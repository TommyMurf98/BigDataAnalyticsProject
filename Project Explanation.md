This was a university assignment/project for the Big Data Analytics module that analyzes COVID-19 time series data from Indonesia, specifically focusing on the number of active cases, new cases per million, and other related metrics. The code is centered around data cleaning, visualization, and statistical analysis of the pandemic's impact across different locations within Indonesia, particularly focusing on DKI Jakarta.

### Here's what the code does:

1. **Imports**:
   - The standard libraries `pandas`, `matplotlib`, and `numpy` are imported for data manipulation and visualization.

2. **Data Loading**:
   - The dataset `covid_19_indonesia_time_series_all.csv` is loaded using `pandas.read_csv()`, and the first few rows are displayed with `head()`.

3. **Data Cleaning**:
   - The data is filtered to remove any rows where "Total Active Cases" is less than 0. The cleaned dataset is saved to a CSV file named `Cleaned_data.csv`.

4. **Data Information**:
   - The `info()` function is called on the cleaned dataset to get an overview of the data structure.

5. **Date Conversion**:
   - The "Date" column is converted to a datetime format using `pd.to_datetime()` to facilitate time-based analysis.

6. **Visualization Setup**:
   - The plot size is set using `matplotlib.rcParams`.

7. **Analyzing Jakarta Data**:
   - The data specific to DKI Jakarta is filtered and stored in `jakarta_data`, and the corresponding dates are stored in `jakarta_dates`.

8. **Plotting New Cases per Million (Jakarta)**:
   - A line plot is generated to visualize the "New Cases per Million" in Jakarta over time, with ticks on the x-axis placed every 60 days.

9. **Plotting Total Active Cases (Jakarta)**:
   - Another line plot is created to show the "Total Active Cases" over time in Jakarta, again with x-axis ticks placed every 60 days.

10. **Statistical Description**:
    - The `describe()` method is used to generate statistical summaries (like mean, median, etc.) for "Total Active Cases" and "New Cases per Million" in Jakarta.

11. **Additional Comments/Ideas**:
    - There are comments in the code indicating attempts to calculate case rates for provinces with populations over 5 million, group data by month and year, and analyze the relationship between population density and case rates.

### Project Overview:
The main focus of the project is to analyze the spread of COVID-19 in Indonesia, with a specific focus on Jakarta. The project visualizes trends in new cases per million and total active cases, provides statistical summaries, and explores the relationship between population and case rates. The user interface is minimal, and the primary output consists of graphs and statistical insights.
