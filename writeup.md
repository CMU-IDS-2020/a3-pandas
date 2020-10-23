# Project name: Air Pollution Study of United States from 2000 to 2016

![A screenshot of your application. Could be a GIF.](screenshot.png)

TODO: Short abstract describing the main goals and how you achieved them.


## Project Goals

TODO: **A clear description of the goals of your project.** Describe the question that you are enabling a user to answer. The question should be compelling and the solution should be focused on helping users achieve their goals. 

The questions user could answer with the application including:
1. What is the trend of four differnt pollutants for different states over time?
2. Which states have the most series problem of different air pollutants?
3. What are the top states/ counties/ cities with most/least serious air pollutant problem?
4. What is the distribution of the max hours of different pollutants for selected state/ county/ city?

## Design

TODO: **A rationale for your design decisions.** How did you choose your particular visual encodings and interaction techniques? What alternatives did you consider and how did you arrive at your ultimate choices?

We provided four types of visual encodings allowing users to explore the U.S air pollution dataset. 
First interactive graph allows user to select measurement, type of pollutant, states, and a range of time. The visualization will then provide the mean of the measurement over the time range that is specified with different colors of line indicating different states. 
The second visualization is a map that contains the mean of the measurement of the selected pollutant for all the states, a highligher is added to allow user view the detailed value for different states. 
The third visualization intend to allow user explore which states, counties and cities are the highest or lowest measurements for different pollutant. This visual component allow user to choose different geographic entities (state, county, city) and the top N entities with either highest or lowest mean measurements for the selected pollutant. The geographic entities are then sorted by the mean 1st Max Value of the selected pollutant. 



## Development

TODO: **An overview of your development process.** Describe how the work was split among the team members. Include a commentary on the development process, including answers to the following questions: Roughly how much time did you spend developing your application (in people-hours)? What aspects took the most time?

## References
Data source: Air Pollution in the U.S. since 2000-2016 https://data.world/data-society/us-air-pollution-data
