# Analysis of Beach Water Quality and Weather Patterns from IoT Sensors

## Title: Analysis of Beach Water Quality and Weather Patterns from IoT Sensors

### Group Members:
- Akhil Kanukula
- Akhil Mittapalli
- Soubhagya Panda

---

## Introduction
The objective of this project is to demonstrate proficiency in utilizing data analysis techniques through the formulation and testing of hypotheses. Using real-world data from IoT sensors monitoring water quality and weather conditions at Chicago beaches, we aim to provide actionable insights. The datasets chosen include weather and water quality information recorded at Chicago beaches, providing a foundation to test hypotheses and evaluate patterns.

---

## Data Sources

### Dataset Links:
1. [Beach Weather Stations - Automated Sensors](https://catalog.data.gov/dataset/beach-weather-stations-automated-sensors)
2. [Beach Water Quality - Automated Sensors](https://catalog.data.gov/dataset/beach-water-quality-automated-sensors)
3. [Beach Water and Weather Sensor Locations](https://data.cityofchicago.org/Parks-Recreation/Beach-Water-and-Weather-Sensor-Locations/g3ip-u8rb/about_data)

### Basic Information About the Data
#### 1. Beach Water Quality Dataset:
- **Rows:** 42.6k
- **Columns:** 10
- **Attributes:** Beach Name, Measurement Timestamp, Water Temperature, Turbidity, Transducer Depth, Wave Height, Wave Period, Battery Life, Measurement Timestamp Label, Measurement ID
- **Size:** 4.5 MB

#### 2. Beach Weather Stations Dataset:
- **Rows:** 171k
- **Columns:** 18
- **Attributes:** Station Name, Measurement Timestamp, Air Temperature, Wet Bulb Temperature, Humidity, Rain Intensity, Interval Rain, Total Rain, Precipitation Type, Wind Direction, Wind Speed, Maximum Wind Speed, Barometric Pressure, Solar Radiation, Heading, Battery Life, Measurement Timestamp Label, Measurement ID
- **Size:** 25.5 MB

#### 3. Sensor Locations Dataset:
- **Rows:** 9
- **Columns:** 5
- **Attributes:** Sensor Name, Sensor Type, Latitude, Longitude, Location
- **Size:** 860 B

---

## Methodology

### Exploratory Data Analysis (EDA)
1. **Data Cleaning:**
   - Removed null values or replaced them with sentinel values or mean values.
   - Renamed columns for consistency (e.g., replacing spaces with underscores).
   - Dropped unused columns to optimize analysis.

2. **Visualizations:**
   - Box plots and violin plots for distribution analysis.
   - Joint and scatter plots to identify relationships.
   - Time-series plots and rolling averages for trend analysis.

3. **Correlation Analysis:**
   - Correlation matrices were generated to understand relationships between variables such as air temperature, humidity, wind speed, water temperature, turbidity, and wave height.

4. **Seasonal Analysis:**
   - Seasonal impacts were analyzed by grouping data into winter, spring, summer, and fall.
   - Wind rose plots were created to understand wind direction patterns.

---

## Hypothesis Testing

### Hypothesis 1:
**Montrose Beach is the best beach to spend time with good weather and water conditions.**

#### Observations:
- **Water Conditions:**
  - Average water temperature: 15-20 °C.
  - Turbidity values: Mostly 0, maximum up to 200 NTU.
  - Wave height: Average 0.2 meters, maximum up to 0.6 meters.

- **Weather Conditions:**
  - Air temperature: Average 10 °C, ranging from 0 to 20 °C.
  - Rain intensity: Mostly 0, maximum 20 mm.
  - Wind speed: Average 4 m/s, maximum 40 m/s.
  - Solar radiation: 0-140 W/m², with most values under 100 W/m².

#### Conclusion:
Compared to standard values, Montrose Beach provides optimal conditions for recreation. This hypothesis is **TRUE**.

### Hypothesis 2:
**There is a significant impact of air temperature, humidity, and wind speed on water conditions (water temperature, turbidity, and wave height).**

#### Observations:
- **Air Temperature:**
  - Moderate positive correlation with water temperature (0.49).
  - Slight negative correlation with wave height (-0.26).

- **Humidity:**
  - Slight positive correlation with turbidity (0.23).
  - Slight negative correlation with water temperature (-0.27).

- **Wind Speed:**
  - Slight positive correlation with wave height (0.29).
  - Slight negative correlation with water temperature (-0.16).

#### Conclusion:
The hypothesis is **partially true**, with air temperature showing a significant impact on water temperature, while other relationships are weaker but noticeable.

### Hypothesis 3:
**Temporal patterns in water conditions (wave height and period) are significantly affected by seasonal changes in weather patterns, particularly wind direction and speed.**

#### Observations:
- **Seasonal Variation:**
  - Wave height shows higher variability in spring and fall.
  - Wave period remains consistent across seasons.

- **Wind Speed and Wave Height:**
  - Spring and fall show a stronger positive correlation.

#### Conclusion:
This hypothesis is **TRUE**, with clear seasonal impacts on wave height and wind conditions.

---

## Conclusion
This project successfully demonstrates the utility of IoT sensor data in analyzing beach weather and water conditions. Hypotheses were tested with strong evidence to support decision-making for recreational and safety planning. Montrose Beach emerged as the best beach based on weather and water conditions, while seasonal and environmental factors showed varying impacts on beach conditions.

