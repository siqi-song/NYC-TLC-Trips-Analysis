# For-Hire Vehicle Trip Records

## Introduction

FHV data includes trip data from high-volume for-hire vehicle bases (bases for companies dispatching 10,000+ trip per day, meaning Uber, Lyft, Via, and Juno), community livery bases, luxury limousine bases, and black car bases.

The TLC began receiving FHV trip data from bases in 2015, but the amount of information that has been provided has changed over time. In 2015, only the dispatching base number, pickup datetime, and the location of the pickup were provided to the TLC. In summer of 2017, the TLC mandated that the companies provide the drop-off date/time and the drop-off location. In 2017, the TLC also started to receive information on shared rides, like those offered in services like Lyft Line and Uber Pool. A trip is only considered shared if it was reserved specially with one of these services. After the high volume license type was created in Feb 2019, a high-volume license number was added. This is an overall identifier for app companies who may have multiple base licenses.

## Data Description

Field Name            | Description
----------------------|-------------------------------------------------
dispatching_base_num  | The TLC Base License Number of the base that dispatched the trip.
pickup_datetime       | The date and time of the trip pick-up.
dropoff_datetime      | The date and time of the trip dropoff.
PULocationID          | TLC Taxi Zone in which the trip began.
DOLocationID          | TLC Taxi Zone in which the trip ended.
SR_Flag               | Indicates if the trip was a part of a shared ride chain offered by a High Volume FHV company (e.g. Uber Pool, Lyft Line). For shared trips, the value is 1. For non-shared rides, this field is null.
