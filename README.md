# AI Energy Manager

Final project for the Building AI course

## Summary

AI program that monitors buildings energy performance, compares buildings to each other and detect faults in them. AI program also gives successions what could be the problem in the building.


## Background

In Finland building use 40 % of the energy and produce 30 % of the CO2 emissions. Although emissions are popular topic now a days, energy cost are a major factor for people and companies. I have been in the energy efficiency field for over 10 years now and in my experience, there is 10 – 20 % saving potential in any building. In some buildings that have an undetected fault in their process the saving potential is even greater. 


## How is it used?

Program would be used by building owners and building maintenance to detect abnormalities in the buildings. Affected people would be directly users/residents of the buildings but indirectly by reducing unnecessary CO2 emissions the entire world.


## Data sources and AI methods
Unfortunately, there is no universal open data available for energy consumption for buildings. In the future there might be an open data source with data from public building owners like municipalities. For the time being all the building owners would have to use their own energy consumption data. For larger municipalities that is hundreds even thousands of building and that might be enough for reliable model. Also energy companies have large pools of data but the accessibility is a big question mark. Usually the main energy meters of buildings are used for basis of billing and the data should be reliable. Other needed data are weather data from national weather forecasting service and the building data. Building data can be little inaccurate sometimes so that should be quality tested.
I would use linear regression where variables are things like outside temperature (hourly data), wind speed (hourly data) and solar radiation (hourly data) from the weather dataset. Other needed variables are building size (area or volume which is more readily available), indoor temperature (usually not that easily available and might need extra sensors. Some buildings have building management systems that can be accessed), year of construction and number of users. Predicted values would be heating and electric energy usage. Program would compare the predicted value to the actual value and inform any variations. Program also compares the different buildings coefficient values to each other and estimates buildings that have abnormal values. If the program could access the building management system even more variables could be used.


## Challenges

Program doesn’t fix the actual faults, that would have to done manually. Also correctly estimating the precise fault could be very hard to do without some very detail monitoring in the building and getting the data from building management system to the AI program could be challenging. Early build of the program could produce a list of faults that fit into the characteristics of the data. List of faults and their detection from data can be taught to the program but can be challenging. One major challenge is lack readily available data but luckily things are developing into the right direction.

## What next?

Next step of the program could be affecting designing of the buildings from the learned data of existing buildings. Program could analyze existing buildings and determine what works and what doesn’t and give directions to the building designers.

