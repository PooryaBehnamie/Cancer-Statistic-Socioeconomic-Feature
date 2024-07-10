# Cancer-Statistic-Socioeconomic-Feature
Employed statistical models to explore the impact of socioeconomic factors on cancer incidence and mortality rates across various U.S. states over a decade.
![Screenshot 2024-07-10 181433](https://github.com/PooryaBehnamie/Cancer-Statistic-Socioeconomic-Feature/assets/169101583/f0c45c5b-6d03-44e5-b3fd-47560294f1f1)

# Project Overview
This project aims to explore the impact of socioeconomic and environmental factors on cancer incidence and mortality rates across various U.S. states over a decade. By leveraging detailed datasets from the CDC and County Health Rankings, the objective is to provide actionable insights for public health strategies, focusing on disparities in cancer outcomes influenced by socioeconomic conditions.

# Data Sources
### [**CDC’s United States Cancer Statistics (USCS)**:](https://wonder.cdc.gov/controller/datarequest/D189;jsessionid=A0BCF1C198428769EAF82199648F?stage=results&action=toggle&p=O_show_rank&v=true)
* Includes registry data from NPCR and SEER programs.
* Covers demographic and tumor characteristics such as age, gender, cancer type, and stage at diagnosis.
* Data spans from January 1, 2001, to December 31, 2020.

### [**County Health Rankings**:](https://www.countyhealthrankings.org/health-data/methodology-and-sources/data-documentation/national-data-documentation-2010-2022)
* Compiled by the University of Wisconsin Population Health Institute.
* Provides information on health outcomes and factors influencing health at the county level, including socioeconomic metrics like income levels, insurance coverage, and lifestyle factors such as smoking rates.

### **GeoJSON File for Map Visualization**:
* The GeoJSON file used for the map visualization in this project was sourced from PublicaMundi's MappingAPI repository. The file contains geographical boundaries that are essential for creating accurate and informative maps.
* You can find and download the GeoJSON file from the following link: [PublicaMundi GeoJSON Data](https://github.com/PublicaMundi/MappingAPI/tree/master/data/geojson).

# Methods and Analysis
#### Data Integration and Cleaning
* Merged cancer incidence and mortality data from the CDC with socioeconomic data from County Health Rankings based on 'State-Year' columns.
* Cleaned and preprocessed the data using pandas to handle missing values, standardize formats, and eliminate duplicates.
#### Exploratory Data Analysis (EDA)
* Conducted EDA to uncover underlying patterns and distributions within the data.
* Generated descriptive statistics to summarize central tendencies, dispersion, and shape of the dataset's distributions.
#### Geospatial Analysis
* Utilized Folium for geospatial mapping to visually represent the data across various U.S. states.
* Created choropleth maps and overlaying circle markers to display incidence and mortality rates of cancer and their association with socioeconomic factors.
#### Cluster Analysis
* Performed K-means clustering to explore how variables such as adult smoking rates, physical inactivity, and mental health provider rates cluster across different states.
* Visualized clusters using seaborn and matplotlib.
#### Statistical Analysis and Model Building
* Applied linear regression to assess relationships between cancer outcomes and individual socioeconomic factors.
* Utilized multiple regression analysis to evaluate the combined impact of various socioeconomic variables on cancer rates.
* Employed cross-validation techniques to assess the model’s performance and stability.
#### Results Interpretation
* Interpreted the coefficients from the regression model, providing insights into how significant each socioeconomic factor is in relation to cancer mortality and incidence rates.
* Discussed the model's mean squared error and R² score to quantify the accuracy and explanatory power of the model.

# Results
* Identified significant correlations such as the link between smoking rates and lung cancer mortality.
* The multiple regression model achieved an R² score of 0.72, indicating a strong explanatory power.
* Findings suggest that lower socioeconomic status and poorer health-related behaviors are closely associated with higher cancer mortality rates.

# Conclusion
The analysis underscores the critical need for targeted public health interventions and policies that address socioeconomic disparities. By mapping the landscape of how social determinants affect cancer outcomes, this study aids in prioritizing efforts to mitigate the impact of the most detrimental factors.

# Report & Visualizations
The project overview and motivation are summarized in a Word report. The report includes detailed descriptions of the data cleaning processes, data sources and collection methods, limitations, biases, and ethical considerations. Additionally, a final presentation for this analysis has been created on Tableau Public. Here is the [link](https://public.tableau.com/views/CancerStatisticSocioeconomicFeature/Story1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) to the visualizations.
