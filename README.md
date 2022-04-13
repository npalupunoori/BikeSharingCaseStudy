# Bike Sharing Case study



## Table of Contents
* [General Info](#general-information)
* [Inital observations](#INITIAL-OBSERVATION)
* [Conclusions](#CONCLUSIONS)
* [Suggestions](#SUGGESTIONS)
* [Contact](#Contact)


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
## INITIAL OBSERVATION
    • Holiday has very low impact on register customers but has a big effect on casual customers. As a result, there is some impact on overall demand.
    • Even though working day does not have impact on overall demand, there is impact on registered and casual customers independently.
    • During summer and winter there is no effect on demand, mostly due to casual customers.
    • January and July there is demand change from registered customers no demand change from casual customers
    • In March and October there is demand change for casual customers but no effect on overall demand.
    • In November there is demand change form registered customers which is affecting overall demand.
    • There is change in demand on Saturday from causal customers that is affecting overall demand.
    • There is change in demand on Wednesday from registered customers, this is not affecting overall demand.

## CONCLUSIONS
    • With no other elements effecting the demand, there is more demand in casual customers then the registered customers.
    • There is a positive demand increase in bikes for both registered and casual customers when it gets warmer.
        * For every 2 units increase in temperature there is 1 unit increase in demand.
    • Demand for bike from casual customers tend to increase in summer. Increase in demand is very significant.
    • Winter has more increase in demand then summer, all the demand increase is from registered customers.
    • There is good increase in demand form registered customers in 2019, there is almost 25% increase in demand
    • On windy days there is obvious drop in demand from all customers.
    • There is loss of customers in snowy and cloudy days.
        * There is drop in demand from registered customers, Casual customers don’t have much effect on demand during this season.
    • Working day has opposite effect on demand from registered and casual customers, drop in demand from casual customers is compensated by demand from registered customers.
    • Humidity as huge effect on casual customer’s demand. Casual customers like to use bike’s when the weather is better.
    • During Sunday’s there is uptick in demand from casual customers.

## SUGGESTIONS
    • Customer service team and supply team need be ready to handle demand increase in warmer days.
    • Marketing team need to focus on getting more casual customers in summer and converting them to register customers, so they continue to become more regular users of bike and keep the demand up in winter also.
    • In general, people are getting more health concussions this might contribute to increase in demand year on year.
    • On working days looks like register customers are using bike sharing for commute to work. So, demand for bikes in residential area might increase during daytime and increase in demand in industrial area during evenings.
        * Marketing team need to focus on having some deals to get more casual customer to use during the evenings, like happy hour.
        * Loss of demand from casual customers is negating the demand increase from registered customers.
        * It is important to get more casual customers on working days.
    • To handle the drop in demand in windy days, company need to think to upgrade to aerodynamic bikes and advertise it accourdingly.



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