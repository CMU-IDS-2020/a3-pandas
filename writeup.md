# Study of Air Pollution in United States from 2000 to 2016
Faner Lin (fanerl), Shuaidong Pan (shuaidop)
![A screenshot of your application. Could be a GIF.](screenshot.png)


Air pollution has become a more and more serious issue. In different studies, it has shown that air pollution will exacebate climate change and could cause different health issues. Different air pollutant could be an important simulus for respiratory disease and cardiovascular disease. Air pollution is a mixture of different components, and some of the main pollutants of great concern includes gaseous ozone, nitrogen dioxide, carbon monoxide, and surphur dioxide. The explored dataset contains the recorded the information of four major pollutant, ozone, nitrogen dioxide, carbon monoxide, and surphur dioxide, for each day from 2000-01-01 to 2016-05-31 for different places in U.S. The visualizations presented in the study could help analyzing trends for different pollutants over time for different states and help identifying states, counties, and cities with serious pollution concerns. Additionally, user could select specific city, county, and state to view the max hour of pollutant measurement over selected time range. The the source of the data has been included at the end of the document and the visualizations and the application are created with Altair and Streamlit. For data preprocessing, exploratory analysis and transformation, we use the package numpy and pandas in Python. 

## Project Goals

The project aims to help user analyze air pollution data in U.S. from 2000 to 2016. The visualization allows flexibility of selecting different pollutant, type of measurements, time range, geographical entities, and others. Some goal for the interactive visualizations presented in the study include help user analyzing trends for different pollutants over time for different states and help identifying states, counties, and cities with serious pollution concerns. Additionally, user could select specific city, county, and state to view the max hour of pollutant measurement over selected time range.
Below are some questions one could answer with the application:
1. What is the trend of four differnt pollutants for different states over time?
2. Which states have the most series problem of different air pollutants?
3. What are the top states/ counties/ cities with most/least serious air pollutant problem?
4. What is the distribution of the max hours of different pollutants for selected state/ county/ city?
5. What hour within a day does the city of Boston has the highest concentration of CO from 2016-01-01 to 2016-01-31?
6. What is the relationships between different 

## Design

We provided four types of visual encodings allowing users to explorep the U.S air pollution dataset. 
The unit for measure four different polllutant NO2, SO2, CO, O3 are Parts per million. There are four different measurements for each pollutant (tabke NO2 as example):
 * Mean: The arithmetic mean of concentration of NO2 within a given day
 * AQI: The calculated air quality index of NO2 within a given day
 * 1st Max Value: The maximum value obtained for NO2 concentration in a given day
 * 1st Max Hour: The hour when the maximum NO2 concentration was recorded in a given day

#### Pollutant Change Over Time
First interactive graph allows user to select one of the first three measurement, type of pollutant, states, time period, and the plotting frequency. For plotting frequency, we offer three different options, yearly, monthly, and daily. The visualization will then provide the aggregated mean of the measurement over the time range given the select plotting frequency for the selected pollutant and measurement. Different colors of line in the plot indicates different states. 

The second interactive graph allows user to check the relationships between different pollutants for a selected state over a selected period of time. Entries coming from different cities are distinguished by different colors. User could choose two different pollutants at the same time. 

#### Pollutants Relationship
The third visualization is a continuation from the first plot: a map that contains the mean of the measurement of the selected pollutant for all the states over the selected period of time, a highligher is added to allow user view the detailed value for different states. 

#### Pollutants Distribution
The fourth visualization intend to allow user explore which states, counties and cities have the highest or lowest measurements for different pollutants. This visual component allow user to choose different geographic entities (state, county, city), the number of entities to show, and the option of plotting highest or lowest mean measurements for the selected pollutant. Three measurements, mean, AQI, and 1st max value, are presented as bars in the graph with different colors. The y-axis indicating the top N geographic entities given the plotting criterias. Moreoever, the geographic entities are then sorted by the mean of the 1st Max Values of the selected pollutant for different geographic entities.

#### Max Hours for Pollutants within a day
The last visualization provide information regarding the hour when the maximum pollutant concentration was recorded in a given day. User could select a geographical entities (state, county, city), and then select a specific region and a period of time. The distribution of the max hour for all four pollutants are then shown, with x-axis representing the hour in a day and y-axis representing the count of the values of the max hours. With the plot, for instance, we could analyze what is the hour in a day that has the highest concentration of CO and O3 for the day of 2016-01-01 for the city of Boston. User could also analyze, for example, what is the most frequent hour such as SO2 will have the highest concentration within a day from 2016-01-01 to 2016-01-31 for the New York City. 


## Development

For the project, Faner and Shuaidong split the work equally and the whole project is a collaboration work with equal participation. Our development process could be roughly divided into three parts: data selection and preprocessing, graphics and visualization desgin, and final deployment and testing. 
For the dataset selection and preprocessing, we spent lots of time browsing different datasets and eventually select the air pollution dataset. We applied data preprocessing techniques and exploratory analysis to understand our dataset. The time we spend on this part is approximately each 8 hours. 
For graphics and visualization design, we first discussed several possible plans according to our exploratory data analysis result and eventually settle down on the ones shown on the application page. We aimed to deliver information efficiently by designing a flexible and multi-functional graph, so users could see from our application that there are many selection box for specifying different inputs. For the graphics and visualization design, we spend around 5 hours constructing and modifying our graphical design and interaction design. 
For final deployment and testing, we spent most of our time. We combined different graphical elements and trying to successfully deploy our model and coding those graphical design with different data transformation and data integration techniques. We spend around 15 hours each on this part. 



## References
Data source: Air Pollution in the U.S. since 2000-2016 https://data.world/data-society/us-air-pollution-data
Expert position paper on air pollution and cardiovascular disease: https://academic.oup.com/eurheartj/article/36/2/83/2293343
Altair documentation page: https://altair-viz.github.io/getting_started/overview.html



