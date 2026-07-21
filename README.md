# Weather Forecast Analysis
## Purpose
This is a collection of jupyter notebooks in which I analyze weather and forecast data to get a better 
idea of the domain of renewable energies and the forecast thereof.  
I want to test the general usage and capabilities of weather APIs, as well as conduct some experiments on the correlation of
sun/cloud and wind forecasts.
## Context
The marketing of renewable energies implies a considerable effort to predict power production one day ahead
of the actual consumption and production. Prediction errors can either cause unsold energy (in case of a low estimate) 
or the need to buy expensive energy on more short-term markets (in case of a too high estimate).  
The aggregation of assets in a portfolio can reduce the insecurity of a prediction, because prediction errors need not linearly sum up.
Wind parks might deliver more energy than thought while assets based on solar energy might deliver less, which is a desirable case of errors cancelling out. 
On the other hand, two solar parks close to each other will produce summed up errors. 
The third case might be assets that are widely unrelated because they are far away from each other:  
Their prediction errors will sum up like the length of two perpendicular vectors.

## First Results
The OpenWeather API delivers a wider variety of weather variables, both historically archived, forecast and, quite important,
archived forecasts.  
First experiments show that the location of assets has a big influence on the correlation of their errors. Cloud estimation 
errors drop under 0.2 in correlation coefficient after ~200km of distance, while wind takes about twice as much. 
Also for some specific locations, negative correlations have been found, which would be very attractive as asset locations. But these relations 
need more research and statistic tests. At first sight, though, a correlation coefficient < -0.2 over a period of more than half a 
year is not a mere coincidence.



 
