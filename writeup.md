# Air Pollution Study of United States from 2000 to 2016
Faner Lin (fanerl), Shuaidong Pan (shuaidop)
![A screenshot of your application. Could be a GIF.](screenshot.png)

TODO: Short abstract describing the main goals and how you achieved them.

Air pollution has become a more and more serious issue. In different studies, it has shown that air pollution will exacebate climate change and could cause different health issues. Different air pollutant could be an important simulus for respiratory disease and cardiovascular disease. Air pollution is a mixture of different components, and some of the main pollutants of great concern includes gaseous ozone, nitrogen dioxide, carbon monoxide, and surphur dioxide. The explored dataset contains the recorded the information of four major pollutant, ozone, nitrogen dioxide, carbon monoxide, and surphur dioxide, for each day from 2000-01-01 to 2016-05-31 for different places in U.S. The visualizations presented in the study could help analyzing trends for different pollutants over time for different states and help identifying states, counties, and cities with serious pollution concerns. Additionally, user could select specific city, county, and state to view the max hour of pollutant measurement over selected time range. The the source of the data has been included at the end of the document and the visualizations and the application are created with Altair and Streamlit. For data preprocessing, exploratory analysis and transformation, we use the package numpy and pandas in Python. 

## Project Goals

TODO: **A clear description of the goals of your project.** Describe the question that you are enabling a user to answer. The question should be compelling and the solution should be focused on helping users achieve their goals. 
The project aims to help user analyze air pollution data in U.S. from 2000 to 2016. The visualization allows flexibility of selecting different pollutant, type of measurements, time range, geographical entities, and others. Some goal for the interactive visualizations presented in the study include help user analyzing trends for different pollutants over time for different states and help identifying states, counties, and cities with serious pollution concerns. Additionally, user could select specific city, county, and state to view the max hour of pollutant measurement over selected time range.
Below are some questions one could answer with the application:
1. What is the trend of four differnt pollutants for different states over time?
2. Which states have the most series problem of different air pollutants?
3. What are the top states/ counties/ cities with most/least serious air pollutant problem?
4. What is the distribution of the max hours of different pollutants for selected state/ county/ city?

## Design

TODO: **A rationale for your design decisions.** How did you choose your particular visual encodings and interaction techniques? What alternatives did you consider and how did you arrive at your ultimate choices?

We provided four types of visual encodings allowing users to explore the U.S air pollution dataset. 
The unit for measure four different polllutant NO2, SO2, CO, O3 are Parts per million. There are four different measurements for each pollutant:

 * Mean: The arithmetic mean of concentration of NO2 within a given day
 * AQI: The calculated air quality index of NO2 within a given day
 * 1st Max Value: The maximum value obtained for NO2 concentration in a given day
 * 1st Max Hour: The hour when the maximum NO2 concentration was recorded in a given day

First interactive graph allows user to select one of the first three measurement, type of pollutant, states, time period, and the plotting frequency. For plotting frequency, we offer three different options, yearly, monthly, and daily. The visualization will then provide the aggregated mean of the measurement over the time range given the select plotting frequency for the selected pollutant and measurement. Different colors of line in the plot indicates different states. 

The second visualization is a continuation from the first plot: a map that contains the mean of the measurement of the selected pollutant for all the states over the selected period of time, a highligher is added to allow user view the detailed value for different states. 

The third visualization intend to allow user explore which states, counties and cities have the highest or lowest measurements for different pollutants. This visual component allow user to choose different geographic entities (state, county, city), the number of entities to show, and the option of plotting highest or lowest mean measurements for the selected pollutant. Three measurements, mean, AQI, and 1st max value, are presented as bars in the graph with different colors. The y-axis indicating the top N geographic entities given the plotting criterias. Moreoever, the geographic entities are then sorted by the mean of the 1st Max Values of the selected pollutant for different geographic entities.




## Development

TODO: **An overview of your development process.** Describe how the work was split among the team members. Include a commentary on the development process, including answers to the following questions: Roughly how much time did you spend developing your application (in people-hours)? What aspects took the most time?

## References
Data source: Air Pollution in the U.S. since 2000-2016 https://data.world/data-society/us-air-pollution-data
