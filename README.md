# NYC TLC Trip Record Data Analysis

This project focuses on analyzing NYC Taxi and Limousine Commission (TLC) trip record data. The goal is to gain insights into various aspects of taxi trips in New York City, such as fare distribution, trip duration, passenger count, and geographical trip patterns. This analysis is crucial for understanding the operational dynamics of taxi services in NYC and can aid in decision-making for improving services and revenue.

## Project Structure

### Files

- AdriHamdi_ProjekModul2.ipynb: The main Jupyter Notebook containing the data analysis and visualizations.

### Data Dictionary

1. *VendorID*: A code indicating the TPEP provider.
   - 1 = Creative Mobile Technologies, LLC
   - 2 = VeriFone Inc.
2. *tpep_pickup_datetime*: The date and time when the meter was engaged.
3. *tpep_dropoff_datetime*: The date and time when the meter was disengaged.
4. *passenger_count*: The number of passengers in the vehicle. This is a driver-entered value.
5. *trip_distance*: The elapsed trip distance in miles reported by the taximeter.
6. *RatecodeID*: The final rate code in effect at the end of the trip.
   - 1 = Standard rate
   - 2 = JFK
   - 3 = Newark
   - 4 = Nassau or Westchester
   - 5 = Negotiated fare
   - 6 = Group ride
7. *store_and_fwd_flag*: This flag indicates whether the trip record was held in vehicle memory before sending to the vendor because the vehicle did not have a connection to the server.
   - Y = store and forward trip
   - N = not a store and forward trip
8. *PULocationID*: TLC Taxi Zone in which the taximeter was engaged.
9. *DOLocationID*: TLC Taxi Zone in which the taximeter was disengaged.
10. *payment_type*: A numeric code signifying how the passenger paid for the trip.
    - 1 = Credit card
    - 2 = Cash
    - 3 = No charge
    - 4 = Dispute
    - 5 = Unknown
    - 6 = Voided trip
11. *fare_amount*: The time-and-distance fare calculated by the meter.
12. *extra*: Miscellaneous extras and surcharges.
    - Includes the $0.50 and $1 rush hour and overnight charges.
13. *MTA_tax*: $0.50 MTA tax that is automatically triggered based on the metered rate in use.
14. *improvement_surcharge*: $0.30 improvement surcharge assessed on hailed trips at the flag drop. The improvement surcharge began being levied in 2015.
15. *tip_amount*: This field is automatically populated for credit card tips. Cash tips are not included.
16. *tolls_amount*: The total amount of all tolls paid in the trip.
17. *total_amount*: The total amount charged to passengers. Does not include cash tips.
18. *trip_type*: A code indicating whether the trip was a street hail or a dispatch.
    - 1 = Street-hail
    - 2 = Dispatch

### Data Cleaning Steps

1. *Remove Unnecessary Columns*: 
   - Columns with all NaN values or irrelevant information were dropped.
2. *Handle Missing Values*:
   - Rows with missing values were removed to ensure data completeness.
3. *Correct Data Types*:
   - Columns were converted to appropriate data types for analysis, such as datetime and numeric formats.
4. *Breakdown DateTime Columns*:
   - Extracted useful features from datetime columns, such as hour, day, and month.

### Analysis Steps

1. *Initial Data Inspection*:
   - Displayed the first few rows and summary statistics to understand the data structure and initial insights.
2. *Data Cleaning*:
   - Performed necessary data cleaning steps to prepare the data for analysis.
3. *Feature Engineering*:
   - Created new features from existing data to enhance analysis, such as trip duration and trip speed.
4. *Data Visualization*:
   - Used various plots and charts to visualize key insights, such as trip distribution, fare amounts, and pickup/drop-off locations.
5. *Statistical Analysis*:
   - Conducted statistical tests and calculated correlations to understand relationships between variables.

### Key Findings

- *High Demand Areas*:
  - Certain locations showed consistently high pickup and drop-off rates, indicating high demand areas.
- *Fare Distribution*:
  - Analyzed fare distribution to understand pricing patterns and fare amounts.
- *Trip Duration*:
  - Examined trip duration patterns to identify peak hours and potential delays.

### Recommendations

1. *Dynamic Pricing*:
   - Implement dynamic pricing based on demand patterns to maximize revenue.
2. *Optimize Fleet Allocation*:
   - Adjust fleet distribution to high-demand areas during peak hours.
3. *Promotional Strategies*:
   - Launch targeted promotions in lower-demand areas to increase usage.

## Conclusion

This analysis provides valuable insights into the operational dynamics of NYC taxi services. By leveraging these insights, taxi service providers can optimize their operations, improve service quality, and increase revenue.

## License

This project is licensed under the MIT License.

## Contact

For any questions or feedback, please contact Adri Hamdi at [hamdiadri88@gmail.com].
