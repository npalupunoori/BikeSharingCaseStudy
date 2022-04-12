# Bike Sharing Case study



## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
=========================================

### Dataset characteristics
=========================================
day.csv have the following fields:

    - instant: record index
    - dteday : date
    - season : season (1:spring, 2:summer, 3:fall, 4:winter)
    - yr : year (0: 2018, 1:2019)
    - mnth : month ( 1 to 12)
    - holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
    - weekday : day of the week
    - workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
    + weathersit : 
        - 1: Clear, Few clouds, Partly cloudy, Partly cloudy
        - 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
        - 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
        - 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
    - temp : temperature in Celsius
    - atemp: feeling temperature in Celsius
    - hum: humidity
    - windspeed: wind speed
    - casual: count of casual users
    - registered: count of registered users
    - cnt: count of total rental bikes including both casual and registered

=========================================


## Conclusions

    - With no change in any parameter there is a uptick in casual coustmers.
    - Temperature has most positive effect on the all coustomers, Even in sub category of REgistered and Casual coustomers. 
        * There might be more demand in day's where temperature is hotter.
    - Windspead has a negative effect, Which makes sense coustomers might not be liking to ride bikes when it is very windy.
        * One way to get more coustomers is get aerodymic bikes which might negate for the windspeed.
    - Summer has very little effect on over all coustomers.
        * There is no change in summer effect.
        * There is little up tick in summer effect.
        * We can also observe, there is up tick in registered coustomers in winters.
        * Casual coustomers tend to not ride in winter.
            * Over all we can observe that there is no uptick in summer, but trend can registered coustomers continue to ride in winter also. So effort needs to put in to get more registered coustomers in summer, Which lead to more coustomers in winter.
        * Snow has a decremental effect on coustomers, We can plan for low demand in winter.
        * Mist and cloud also has a decremental effect, One of the things to improve and reduce the effect of mist can be to get soloar light bikes so the vissibility gets better in mist conditions.
    - Year to year there is up tick in coustomers, there is good increment in registered cousomters. Need to run some schemas for casual cosutomers to attrack them to ride bikes. 
        * Attarack more casual coustomers and convert them to registered coustomers.
        * There will be small uptick in demand for registered bikes in sepetember. 
            - We can anticipate the up tick in september by having a look at registered coustomers.
    - Working day has a negative effect on casual coustomers, May be run some discounts or speal deals for casual riders on working day's
        * Rush hour deals for casual coustomers.
    - There will drop in demand on humid days, we can use these days for bike servicing. Looking at the models above, Shows that humidity has negative effect on all coustomers.
    - October has a up tick in casual rides, this might be due to start of fall, customers want to enjoy the fall colors.
    - Casual works tend to ride more on sunday's. To attract more coustmers on sunday, run some deals for the casual deals.


## Contact
Created by [@npalupunoori] - feel free to contact me!

## License
=========================================
Use of this dataset in publications must be cited to the following publication:

[1] Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.

@article{
	year={2013},
	issn={2192-6352},
	journal={Progress in Artificial Intelligence},
	doi={10.1007/s13748-013-0040-3},
	title={Event labeling combining ensemble detectors and background knowledge},
	url={http://dx.doi.org/10.1007/s13748-013-0040-3},
	publisher={Springer Berlin Heidelberg},
	keywords={Event labeling; Event detection; Ensemble learning; Background knowledge},
	author={Fanaee-T, Hadi and Gama, Joao},
	pages={1-15}
}

=========================================