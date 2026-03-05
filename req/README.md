# Palmetto Machine Learning: Software Engineering Assignment

## Problem Statement

You are tasked with building a simple API that provides benchmarks for monthly electricity consumption of single-family homes in California. The API must take in a home's location as latitude and longitude coordinates, and return a baseline time series of 12 monthly values. These baselines are defined as the average electricity consumption for that location's county. We are interested in your approach to data wrangling, API development, and deployment.


## Data Sources

* `building_characteristics.csv`: tabulates building characteristics for a sample of 332 single-family homes in California. Importantly, this dataset identifies the county of each building. This sample can be deemed as representative of the population of single-family homes in California.

* `electricity_consumption.csv`: contains the _daily_ electricity consumption in kWh for every building in `building_characteristics.csv`.

* `counties.geojson`: contains the geographical boundaries, in WGS84 coordinates, of each county in California.

## Objectives
1. **Wrangle**: Write a script to ingest the provided data, compute monthly electricity consumption for each county in California, and save the results in a format or database system of your choosing.
    * Thoroughly document each step, and ensure your data transformations are reproducible.
    * You may use any language, tool, or library you see fit. (Python is preferred)
    * Even though this data is small, consider choosing an approach and architecture that would scale to larger datasets.
2. **Develop**: Make this data consumable through an API endpoint.
    * The API must resolve the latitude and longitude coordinates to a county, and return the average monthly electricity consumption for that county.
    * You may use any web framework, library, or tool you see fit. (Python is preferred)
    * Bonus points for careful consideration of error handling, data validation, and testing.
3. **Deploy**: Document how to run a releasable version of the API.
    * The API should be accessible on `localhost` after following your instructions.
    * Consider packaging the API in a containerized environment (Docker preferred).
4. **Discuss**: For a potential follow-up interview, be prepared to discuss your architecture decisions, as well as future improvements, scalability, and maintainability. Specifically be prepared to discuss how your solution might change if the API were to accept location _and_ building characterisitcs, and serve predicted electricity consumption.


## Delivery
Please submit a zipped folder containing all the data, code, and documentation. Structure the folder as you would a git repository. Include a README file with instructions on how to run the API. If you used a coding assistant like Claude, Cursor, Codex, etc, please include the prompts you used along the way, along with any skills or context files that influenced the work.
