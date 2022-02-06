# Flight Delays and Cancellations for the years 1988, 1998 and 2008
## by Basel Zayyat


## Dataset

The complete data set consists of flight arrival and departure details for all commercial flights
within the USA, from October 1987 to April 2008.
As the original dataset is ~120MM records and for the purposes of the analysis, this analysis will
be limited to 3 years (1988,1998, and 2008).
The choice of the years considered a systematic sample where an interval of 10 years was
chosen to represent the sample population.
The data was downloaded from the American Statistical Association from here
(http://ww2.amstat.org/sections/graphics/datasets/DataExpo2009.zip)
where the original data set is collected by The data is collected by the Office of Airline
Information, Bureau of Transportation Statistics (BTS), United States Department of
Transportation. The original data set can be found here
(https://www.transtats.bts.gov/DatabaseInfo.asp?QO_VQ=EFD&Yv0x=D)
The chosen sample contains 17,596,545 rows and represents ~ 15% of the total available data
set with 29 columns.

The aim of this study is to better understand the attributes contributing to delays and
cancellations of flights. 
for the purposes of this study a flight is considered delayed when it is 15
minutes later than its scheduled time and cancellation occurs when the airline does not operate
the flight at all for a certain reason as per the The Federal Aviation Administration (FAA), details
can be found here (https://en.wikipedia.org/wiki/Flight_cancellation_and_delay)
The sample dataset was further reduced into a subset that captures delays equal to or greater
than 15 minutes and cancelled flights generating 4,400,236 rows and 29 columns for the
analysis. This subset was saved as 'd_c_flights.csv' in the project folder.

The subset was produced by wrangling the chosen sample set to include delayed or cancelled flights as per the delay definition.
The Scheduled departure and arrival times were reduced to hours for the purposes of this analysis. 

## Summary of Findings

Multiple delay and cancellation factors were explored. However, it is to be noted that the chosen
subset only included delayed and cancelled flights and not the full flight data set due to system
limitations, hence, the findings are limited to the study subset of cancelled and delayed flights
and could present a biased view. The study subset is also assumed to represent and model the
behaviour of over 3 decades of flying through the selection of the years 1988, 1998, and 2008 as
a representative selective sample.

The univariate exploration included relationships between :

Carriers and the total number of delays/cancellations: for the study period, during which it
was observed that the worst three carriers in terms of the numbers of cancellations are
Southwest, United Airlines and American Airlines
Airports and the total number of delays/cancellations: through which it was established that
flights departing from or landing into Orlando are more likely to suffer from delays or
cancellations

- Day of the week, day of the month, scheduled departure time, and scheduled arrival time
:Fridays, day 22 of the month and departing between 4 to 7 PM or landing between 7 to 9
PM a traveller is more likely to suffer from delays or cancellations

- Cancellation by code:Cancellation by Carrier and National Aviation System (non-extreme
weather conditions, airport operations, heavy traffic volume, and air traffic control) are the
top two reasons for flight cancellations

- Airtime and delays: flights shorter than 50 minutes of Air Time are more likely to experience
delays or cancellation

- Tail number / flight number and total number of cancellations: United Airline appears to take
the top 10 spots in terms of total delays and cancellations grouped by tail number with flight
numbers 419, 65 and 343 suffering above average delays and cancellations.

The bivariate exploration included relationships between :

- Scheduled departure time and scheduled arrival time: for which a linear relationship was
observed were a delay on one side causes a delay on the other.

- Scheduled arrival delays and Airtime: were it was observed that plans are able to recover
delays as air time increases.

- Taxi out time vs. departure delay and taxi in time vs. arrival delay: delayed departures
received preference in terms of taxi timings while this preference was not provided on arrival
as a taxi in preference.

The multivariate exploration included relationships between :

- Month, day of the month and mean delays: July the 13th pops as the day of highest mean
delays.

- Month, day of the week and mean delays: July Sunday's has the max mean delays
Month, day of the month and total cancellations: July 1 has had the most cancellations over
the study period.

- Month, day of the week and total cancellations: January Thursday's appear to suffer the
highest number of cancellatoins.

- Month, scheduled departure time, total delays(departure/arrival max): 16:00 to 19:00
appears to be the period being hit the hradest with delays, with red eye flights showing


## Key Insights for Presentation

This investigation was targeted at identifying the main drivers for delays and cancellations in order to be able to provide recommendations for the least impact of flight delays and cancellations. 

It was observed that travellers flying Southwest, United Airlines and American Airlines, have suffered the most delays with the peak of delays concentrated between the hours 16:00 to 19:00 - a time window to avoid.

Orlando, Atlanta and Dallas airports seem to be the most congested airports.


The top 10 planes impacted by delays and cancellations were United Airlines planes with the flight numbers 419, 65 and 343 suffering above average delays and cancellations

July appears to suffer the most with July 13th having the highest mean delays, July Sunday's having the maximum mean delay and July 1 having the greatest amount cancllations over the study period.