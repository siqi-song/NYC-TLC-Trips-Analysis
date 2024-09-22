# NYC-TLC-Trips-Analysis

Analysis on New York City Taxi &amp; Limousine Commission trip record datasets

All the datasets being used in this project are downloaded from NYC [TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page) site. Only recent records in 2024 (Jan - Jul) are adopted.

Please refer to [TLC Trip Records User Guide](https://www.nyc.gov/assets/tlc/downloads/pdf/trip_record_user_guide.pdf) on how to use the datasets.

The site contains datasets for 4 types of taxis / for-hire vehicles (FHV):
- [Yellow Taxi Trip Records](dictionary/yellow_taxi.md)
- [Green Taxi Trip Records](dictionary/green_taxi.md)
- [For-Hire Vehicle Trip Records](dictionary/for_hire_vehicle.md)
- [High Volume For-Hire Vehicle Trip Records](dictionary/high_volume_for_hire_vehicle.md)

Please click on the links above to understand the details of each dataset.

**[Note]:** All the datasets contain pickup &amp; dropoff Location ID fields. The mappings between Location ID and Borough, Zone, Service Zone could be found in the [Taxi Zone Lookup Table](https://d37ci6vzurychx.cloudfront.net/misc/taxi_zone_lookup.csv).
<br>
*Examples:*
LocationID | Borough       | Zone                    | service_zone
-----------|---------------|-------------------------|----------------
1          | EWR           | Newark Airport          | EWR
2          | Queens        | Jamaica Bay             | Boro Zone
3          | Bronx         | Allerton/Pelham Gardens | Boro Zone
4          | Manhattan     | Alphabet City           | Yellow Zone
5          | Staten Island | Arden Heights           | Boro Zone

Analysis is performed on each type of dataset, and comparisons are also conducted across various taxi/FHV types. Data Analytics results are shown in the respective Python notebooks, and they are also presented in the Markdown files for easy reference:
- [Yellow Taxi Results](results/yellow_taxi_results.md)
- [Green Taxi Results](results/green_taxi_results.md)
- [For-Hire Vehicle Results](results/fhv_results.md)
- [High Volume For-Hire Vehicle Results](results/hv_fhv_results.md)
- [Cross-Taxi Evaluation Results]() [coming soon]

\<WIP\> Include PowerBI file for visualization

\<WIP\> Add ML models training and evaluation sections
