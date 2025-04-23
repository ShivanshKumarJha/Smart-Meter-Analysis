# Smart Meter Analysis Dashboard

This project is a data analysis and visualization dashboard for smart meter data. It processes power consumption data from multiple sources, performs statistical analysis, and generates insightful visualizations to understand energy usage patterns.

## Features

1. **Data Aggregation**:

   - Combines multiple `.xlsx` files from different folders into a single CSV file for each folder.
   - Merges all folder-level CSV files into a single consolidated dataset (`all_etaj_merged_data.csv`).

2. **Descriptive Statistics**:

   - Calculates key statistics (mean, minimum, maximum) for power consumption.
   - Visualizes these statistics using bar charts.

3. **Time-Based Analysis**:

   - Categorizes power consumption data into time periods (Morning, Afternoon, Evening, Night, Midnight).
   - Analyzes and visualizes the occurrences of minimum and maximum power consumption across time periods.

4. **Day-Wise Analysis**:

   - Computes and visualizes the average power consumption for each day of the week.
   - Highlights trends such as higher consumption on weekdays compared to weekends.

5. **Month-Wise Analysis**:
   - Computes and visualizes the average power consumption for each month.
   - Identifies seasonal trends and highlights missing data.

## Visualizations

- **Descriptive Statistics**: Bar chart showing mean, minimum, and maximum power consumption.
- **Time Period Analysis**: Bar charts for minimum and maximum power consumption occurrences by time period.
- **Day-Wise Analysis**: Line chart showing average power consumption for each day of the week.
- **Month-Wise Analysis**: Bar chart showing average power consumption for each month.

## Key Observations

1. **Day-Wise Trends**:

   - Highest average power consumption occurs on **Monday**.
   - Lowest average power consumption occurs on **Saturday**.
   - Weekdays generally show higher consumption compared to weekends.

2. **Month-Wise Trends**:

   - Highest average power consumption occurs in **January**.
   - Lowest average power consumption occurs in **March**.
   - Seasonal trends indicate higher consumption in winter months and during peak summer.

3. **Time Period Analysis**:
   - Minimum power consumption is predominantly observed in the **Morning**.
   - Maximum power consumption occurs exclusively during **Midnight**.

## How to Use

1. **Run the Notebook**:

   - Open `dashboard.ipynb` in Jupyter Notebook or any compatible IDE.
   - Execute the cells sequentially to process the data and generate visualizations.

2. **Output**:
   - The consolidated dataset will be saved as `all_etaj_merged_data.csv`.
   - Visualizations will be displayed inline in the notebook.

## Requirements

- Python 3.x
- Libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `glob`

## File Structure

Smart Meter Anlaysis
├── [.gitignore](.gitignore)
├─] all_etaj_merged_data.csv (ignored)
├── [dashboard.ipynb](dashboard.ipynb)
├─] Etaj 1/ (ignored)
├─] Etaj 2/ (ignored)
├─] Etaj 3/ (ignored)
├─] Etaj 4/ (ignored)
├─] Etaj 5/ (ignored)
├─] etaj1_merged_data.csv (ignored)
├─] etaj2_merged_data.csv (ignored)
├─] etaj3_merged_data.csv (ignored)
├─] etaj4_merged_data.csv (ignored)
├─] etaj5_merged_data.csv (ignored)
├── Output/
│ ├── [descriptiveStats.png](Output/descriptiveStats.png)
│ ├── [minMaxVariations.png](Output/minMaxVariations.png)
│ ├── [MonthlyPowerConsumption.png](Output/monthlyPowerConsumption.png)
│ └── [weeklyPowerConsumption.png](Output/weeklyPowerConsumption.png)
└── README.md