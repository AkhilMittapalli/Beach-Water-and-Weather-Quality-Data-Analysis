Analysis of Beach Water Quality and Weather Patterns from IoT Sensors
Project Overview
This project analyzes the water quality and weather patterns at Chicago beaches using IoT sensor data. By combining datasets of weather, water quality, and sensor locations, we aim to test hypotheses about environmental conditions and their interplay at these beaches. The analysis involves data cleaning, integration, and hypothesis testing using statistical and visualization techniques.

Group Members
Akhil Kanukula
Akhil Mittapalli
Soubhagya Panda
Objective
To demonstrate proficiency in data analysis techniques by formulating and testing hypotheses based on the Chicago beach water quality and weather datasets.

Datasets Used
1. Beach Water Quality Dataset
Description: Provides detailed information about water quality at Chicago beaches.
Size: 4.5 MB
Attributes:
Beach Name
Measurement Timestamp
Water Temperature
Turbidity
Transducer Depth
Wave Height
Wave Period
Battery Life
Measurement Timestamp Label
Measurement ID
Link: Beach Water Quality Automated Sensors
2. Beach Weather Stations Dataset
Description: Contains weather-related data from IoT sensors installed at Chicago beaches.
Size: 25.5 MB
Attributes:
Station Name
Measurement Timestamp
Air Temperature
Wet Bulb Temperature
Humidity
Rain Intensity
Interval Rain
Total Rain
Precipitation Type
Wind Direction
Wind Speed
Maximum Wind Speed
Barometric Pressure
Solar Radiation
Heading
Battery Life
Measurement Timestamp Label
Measurement ID
Link: Beach Weather Stations Automated Sensors
3. Beach Water and Weather Sensor Locations Dataset
Description: Provides location data that links weather and water quality datasets.
Size: 860 B
Attributes:
Sensor Name
Sensor Type
Latitude
Longitude
Location
Link: Beach Water and Weather Sensor Locations
Hypotheses
Hypothesis 1
Montrose Beach is the best beach to spend time at, considering favorable weather and water conditions.

Hypothesis 2
Air temperature, humidity, and wind speed significantly impact water conditions, including water temperature, turbidity, and wave height.

Hypothesis 3
Temporal patterns in water conditions (wave height and wave period) are significantly affected by seasonal weather changes, particularly wind direction and speed.

Data Source and Licensing
The datasets used in this project are publicly available on data.gov and data.cityofchicago.org. These datasets are free for research and analysis purposes without restrictions.

Citations
Beach Water Quality Dataset
Beach Weather Stations Dataset
Beach Sensor Locations Dataset
Getting Started
Prerequisites
Python 3.7 or higher
Required Libraries: pandas, numpy, matplotlib, seaborn, scipy
Steps
Clone the repository.
bash
Copy code
git clone <repository-url>
Download the datasets from the provided links and place them in the data/ folder.
Run the Jupyter Notebook or Python scripts in the analysis/ directory to perform data cleaning, visualization, and hypothesis testing.
Project Structure
kotlin
Copy code
project/
├── README.md
├── data/
│   ├── beach_water_quality.csv
│   ├── beach_weather_stations.csv
│   └── sensor_locations.csv
├── analysis/
│   ├── data_cleaning.ipynb
│   ├── hypothesis_testing.ipynb
│   └── visualizations.ipynb
└── results/
    ├── cleaned_data/
    ├── plots/
    └── hypothesis_results.csv
Acknowledgments
We thank the Chicago Park District and open data platforms for providing IoT-based datasets that made this analysis possible.
