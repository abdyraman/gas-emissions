# gas-emissions
This code is a Python script that analyzes and visualizes data related to CO2 emissions and the percentage of the population living below the poverty line for various countries over a specific time period. Here's what the code does step by step:

1. It imports the necessary libraries, including pandas, numpy, matplotlib, seaborn, and Plotly Express for data manipulation and visualization.

2. It loads two CSV files into pandas DataFrames, `base_df` and `base_df2`, which contain data related to CO2 emissions and poverty rates for various countries.

3. The script then extracts relevant columns from `base_df` and `base_df2` to create two new DataFrames, `df` and `df_poverty`, respectively. These DataFrames are filtered to remove irrelevant rows and any rows with null values.

4. `df` and `df_poverty` are further filtered to create `df_range` and `df_pov_range`, respectively, which contain data for the years between 1990 and 2019.

5. The code merges `df_range` and `df_pov_range` based on the 'country' and 'year' columns, creating a new DataFrame called `df_combined`. This combined DataFrame contains information about CO2 emissions and poverty rates for the selected years and countries.

6. The script then uses Plotly Express to create three different types of visualizations:
   - A line chart that shows CO2 emissions over time for different countries.
   - Another line chart that visualizes the percentage of the population below the poverty line over time for different countries.
   - A scatter plot for the year 2019, which shows the relationship between CO2 emissions and the percentage of the population below the poverty line.

7. The script defines a function called `plot_data_for_country` that takes a DataFrame and a country name as input and creates a dual-axis line chart to visualize CO2 emissions and poverty rates for the specified country over time. It then uses this function to plot data for several countries, such as the United States, China, Germany, the United Kingdom, Canada, Angola, Kyrgyzstan, Kazakhstan, Tajikistan, Uzbekistan, Ukraine, and Russia.

In summary, this code loads and preprocesses data related to CO2 emissions and poverty rates, merges the data, and creates various visualizations to explore the relationship between these two factors for different countries over a specific time range. It also includes a function to plot the data for individual countries.
