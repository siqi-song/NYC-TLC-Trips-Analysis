# Yellow Taxi Trip Records

## Introduction

Trips made by New York City’s iconic yellow taxis have been recorded and provided to the TLC since 2009. Yellow taxis are traditionally hailed by signaling to a driver who is on duty and seeking a passenger (street hail), but now they may also be hailed using an e-hail app like Curb or Arro. Yellow taxis are the only vehicles permitted to respond to a street hail from a passenger in all five boroughs.

Records include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts. The records were collected and provided to the NYC Taxi and Limousine Commission (TLC) by technology service providers. The trip data was not created by the TLC, and TLC cannot guarantee their accuracy.

## Data Description

Field Name            | Description
----------------------|-------------------------------------------------
VendorID              | A code indicating the TPEP provider that provided the record.<br>1 = Creative Mobile Technologies, LLC<br>2 = VeriFone Inc
tpep_pickup_datetime  | The date and time when the meter was engaged.
tpep_dropoff_datetime | The date and time when the meter was disengaged.
passenger_count       | The number of passengers in the vehicle. This is a driver-entered value.
trip_distance         | The elapsed trip distance in miles reported by the taximeter.
PULocationID          | TLC Taxi Zone in which the taximeter was engaged.
DOLocationID          | TLC Taxi Zone in which the taximeter was disengaged.
RatecodeID            | The final rate code in effect at the end of the trip.<br>1 = Standard rate<br>2 = JFK<br>3 = Newark<br>4 = Nassau or Westchester<br>5 = Negotiated fare<br>6 = Group ride
store_and_fwd_flag    | This flag indicates whether the trip record was held in vehicle memory before sending to the vendor, aka "store and forward", because the vehicle did not have a connection to the server.<br>Y = store and forward trip<br>N = not a store and forward trip
payment_type          | A numeric code signifying how the passenger paid for the trip.<br>1 = Credit card<br>2 = Cash<br>3 = No charge<br>4 = Dispute<br>5 = Unknown<br>6 = Voided trip
fare_amount           | The time-and-distance fare calculated by the meter.
extra                 | Miscellaneous extras and surcharges. Currently, this only includes the $0.50 and $1 rush hour and overnight charges.
mta_tax               | $0.50 MTA tax that is automatically triggered based on the metered rate in use.
improvement_surcharge | $0.30 improvement surcharge assessed trips at the flag drop. The improvement surcharge began being levied in 2015.
tip_amount            | Tip amount – This field is automatically populated for credit card tips. Cash tips are not included.
tolls_amount          | Total amount of all tolls paid in trip.
total_amount          | The total amount charged to passengers. Does not include cash tips.
congestion_surcharge  | Total amount collected in trip for NYS congestion surcharge.
Airport_fee           | $1.25 for pick up only at LaGuardia and John F. Kennedy Airports
