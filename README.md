# Weather-Crop-Yield

# Impact of Temperature Fluctuations on Crop Yield in California

## Overview
This project examines the impact of temperature and precipitation fluctuations on agricultural production in California over the past two decades. Utilizing large datasets detailing daily weather summaries and crop yields, the research focuses on understanding the correlation between climate variables and the yield of major crops.

## Project Objectives
The primary objective of this project was to integrate and analyze multiple large datasets related to climate and agriculture, employing a variety of programming languages, environments, and database systems. Specifically, the project aimed to:
1. Utilize at least two datasets, including a semi-structured dataset.
2. Programmatically store and process these datasets in appropriate databases.
3. Perform pre-processing, transformation, analysis, and visualization of the data.
4. Store the processed data in databases for further analysis.

## Datasets
Weather Data: Daily summaries of temperature and precipitation were obtained from the National Centers for Environmental Information (NCEI) API. This data was stored in a MongoDB database, suitable for handling semi-structured data.
Crop Yield Data: Crop yield data was sourced from the Food and Agriculture Organization (FAO), specifically from the FAOSTAT. This structured dataset was stored in a PostgreSQL database.

## Methodology

### Data Acquisition and Storage
- Weather Data: Accessed programmatically using the NCEI API, this data was stored in MongoDB. An ETL (Extract, Transform, Load) pipeline was implemented to clean the data, removing null values and irrelevant fields, and converting necessary fields to appropriate data types for analysis.
- Crop Yield Data: Retrieved from FAOSTAT, the dataset focused on crop yields in California from 2003 to 2022. The data was cleaned, formatted, and stored in PostgreSQL.
### Data Processing
The project involved merging the two datasets on a common field (year), enabling a comprehensive analysis of the relationship between climate variables and crop yields.

### Analysis and Visualization
- Data analysis and visualization were conducted using Python, specifically in the Jupyter Notebook environment. The Seaborn and Matplotlib libraries were used to create visualizations, including:
- Scatter Plots: To explore the relationship between crop yield and average precipitation.
- Histograms and Line Plots: To analyze the distribution and trends in crop yields over time.
- Correlation Matrix: To identify the relationships between various climate variables (temperature, precipitation) and crop yields.

## Results
The analysis highlighted several key findings:
- Negative Correlation with Precipitation: A weak negative correlation was observed between average precipitation and crop yield, suggesting a potential threshold beyond which additional precipitation does not significantly benefit yields.
- Positive Correlation with Temperature: There was a weak positive correlation between average temperature and crop yield, indicating a slight positive effect of rising temperatures on yields, although this relationship is non-linear and can be influenced by extreme weather events.

## Technologies and Tools Used
- Programming Languages: Python was the primary language used for data processing and analysis.
- Databases: MongoDB was used for storing weather data, and PostgreSQL was used for crop yield data.
- Data Analysis and Visualization: The analysis and visualization tasks were carried out using Jupyter Notebook, with Seaborn and Matplotlib libraries.
- Data Storage and Management: Ubuntu Terminal facilitated server management, MongoDB Compass provided a graphical interface for MongoDB, and PG Admin 4 was used for managing PostgreSQL.

