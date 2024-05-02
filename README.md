# Environmental Data Visualization Application

**Team members**: Anastasiia Saenko, Antara Bhide, Keon Nartey

## Idea Description:
This project aims to visualise environmental, specifically pollution related data in [India](https://www.nytimes.com/2017/02/14/world/asia/indias-air-pollution-rivals-china-as-worlds-deadliest.html?_r=0).  

In 2019, as part of a worldwide survey, it was discovered that 21 out of the 30 most polluted cities were in India. And this pushed India’s ranking as a country to 5th place. The US AQI number averaged out at 152 and the PM2.5 figure recorded was 58.08µg/m³. This concentration was 5 times higher than that recommended by the World Health Organisation (WHO). This is an overall improvement on the 2018 figure of 72.54µg/m³. This means serious health problems for most of the country.

The levels of the pollutant PM 2.5 are often well above the World Health Organisation’s recommended level of exposure (often over 5 times higher) and this leads to serious respiratory problem for those exposed to it. This is from both outside and household air pollution. Records show that in 2019 over 1.6 million deaths were attributed to poor air quality. the State of Global Air 2020 noted that air pollution is now the largest risk factor for death amongst all other forms.

In this project, we focus primarily on the pollutants - Sulphur Dioxide and Nitrogen Oxide by analysing their state wise levels. 



## Data 

We wanted to understand more about India’s air quality using quantitative means.

To load the data which is a `csv` and have an what attributes the data has in our module,

First load a python script

> -  From cleaning_data import Environment
> - env = Environment("../data/data.csv") where you specify the path to the data in the object class.

The two of the 4 dangerous gas over the years in India has been Sulphur Dioxide (SO2) and Nitrogen oxide (NO2) we wanted to get the average levels these gases in india over the period.

Some basic python methods were created to get the 
- mean SO2 levels 
> - `env.average_sulphur_dioxide() = 10.829414322672587`

- mean NO2 levels 
> - `env.average_nitrogen_oxide() = 25.80962289781126`

- get the max SO2 levels by states in India.
> - `environment.state_max_so2()`

## Visualisations

We have included two visualisations our data:

Heatmap : 

We created a heatmap  displaying the average levels of a particular pollutant across different states and years. It visually represents how pollution varies geographically and over time, helping us understand environmental trends and potential health implications more
intuitively. 

  2)  Pie Chart :

The pie chart visually represents the distribution of maximum Sulfur Dioxide (SO2) production across different states. Each slice of the pie corresponds to a state, with the size of the slice indicating the proportion of SO2 production from that state relative to the total production. This provides insights into which states contribute the most to overall SO2 emissions.

The function that was used to generate this pie chart was the `state_max_so2` which we had included in our codebase. The data frame that emeged a s result of this function was visualised as this pie chart. 

## References

https://www.iqair.com/india

https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9189448/




