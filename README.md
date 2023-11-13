# NYC Vehicle for Hire Data Analysis and ML Model

## Project Overview
This project focuses on analyzing the New York City 'Taxi Data', specifically vehicle-for-hire (Uber/Lyft) data from January 1, 2022, to August 31, 2023. The project (will) encompasses a comprehensive statistical analysis followed by the development of a machine learning model. The model is intended for open use, allowing anyone to leverage our insights and predictions.

## Current Project Status
- Finished exploratory ETL (Extract, Transform, Load) process
  [x] Downloaded raw data
  [x] Cleaned and preprocessed the data
  [/] Conducted preliminary measures and analysis

## File Structure
- `ETL_analysis.ipynb`: Jupyter notebook containing the ETL process, initial data exploration to come.

## Getting Started
To use this project, clone the repository and ensure you have the required dependencies installed.

### Prerequisites
- Python 3.x
- Jupyter Notebook
- Dask
- Matplotlib

## Core Data
- Currently not hosted, please reach out for full dataset (7 Gb)
- 
## Usage
Open the `ETL_analysis.ipynb` notebook in Jupyter to view the ETL process and initial data analyses.

## Data Dictonary
| Field              | Data Type         | Description                                                                                         |
| ------------------ | ----------------- | --------------------------------------------------------------------------------------------------- |
| Field              | Data Type         | Description                                                                                         |
| Business           | Object            | Vehicle-for-Hire company operating the ride. Options include Juno, Uber, Via, Lyft.                 |
| Pickup Location    | Integer (64-bit)  | The Taxi and Limousine Commission (TLC) Taxi Zone where the journey commenced. Refer to 'taxi_zone_lookup.csv' for details. |
| Dropoff Location   | Integer (64-bit)  | The TLC Taxi Zone where the journey concluded. Reference 'taxi_zone_lookup.csv' for more information. |
| Trip Length        | Floating point 64 | The total distance of the trip in miles.                                                            |
| Request to Dropoff | Time Delta (ns)   | The time elapsed from the ride request to the dropoff, representing the total time from the passenger's perspective. |
| Request to Pickup  | Time Delta (ns)   | The time taken from the ride request to the passenger pickup.                                       |
| Total Ride Time    | Time Delta (ns)   | The duration between the passenger pickup and dropoff, indicating the total time spent in the car.  |
| On Scene to Pickup | Time Delta (ns)   | The time duration between the driver's arrival on the scene and the passenger pickup, reflecting how long the driver waited. |
| On Scene to Dropoff| Time Delta (ns)   | Time from the driver's arrival on the scene to the passenger dropoff, indicating the driver's total time commitment for the passenger. |
| Time of Day        | Object            | Categorization of the time of day as morning (0600-1100), afternoon (1200-1600), evening (1700-1900), or night (other times). |
| Date               | Object            | The date when the ride was requested.                                                              |
| Hour of Day        | Integer (32-bit)  | The hour of the day when the ride was requested, where 0 represents midnight and 23 represents 11 PM. |
| Week of Year       | Unsigned Integer (32-bit) | The ISO week number of the year when the ride was requested.                                    |
| Month of Year      | Integer (32-bit)  | The ISO month number of the year when the ride was requested, with January as 1.                    |
| Passenger Fare     | Floating point 64 | The total fare paid by the passenger in USD, inclusive of all charges such as base fare, tips, tolls, taxes, surcharges, and applicable fees. |
| Driver Total Pay   | Floating point 64 | The complete payment received by the driver, encompassing base pay and tips.                        |
| Rideshare Profit   | Floating point 64 | The difference between the passenger fare and the driver's total pay, representing the platform's profit. |
| Hourly Rate        | Floating point 64 | The calculated hourly rate based on 'on_scene_hours', including the duration from the driver's arrival to the final drop-off. |
| Dollars per Mile   | Floating point 64 | The driver's earnings per mile, calculated as the total driver pay divided by the trip length.       |


## Contributing
Contributions to this project are welcome. Please follow these steps:
1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a pull request

## License
Distributed under the GNU License. See `LICENSE` for more information.

## Contact
Aaron Weymouth - aaronsweymouth@gmail.com
Project Link: https://github.com/aweymouth13/rideshare_analysis

## Acknowledgements
- NYC Open Data

