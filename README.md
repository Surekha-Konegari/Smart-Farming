# 🌾 Smart-Farming

## 📌 Project Overview

This project seamlessly integrates Machine Learning (RapidMiner) with Data Visualization (Power BI) to drive smarter, data-backed decisions in agriculture. 

Using the Smart Farming Sensor Data for Yield Prediction dataset from Kaggle, RapidMiner builds a Random Forest–based model to accurately forecast crop yield from soil, climate, and farm management parameters. Power BI then transforms these predictions into dynamic, interactive dashboards that reveal actionable farming insights, enabling better resource allocation, risk reduction, and productivity optimization.

## 🎯 Problem Statement

Modern agriculture faces critical challenges such as unpredictable climate conditions, inefficient resource utilization, limited adoption of real-time analytics.

Farmers often rely on experience rather than data-backed insights, leading to suboptimal yields and higher costs. This project bridges that gap by combining predictive analytics with dynamic dashboards, helping stakeholders optimize productivity, resource use, and sustainability.

## 🛠 Tools & Technologies

RapidMiner – Data preprocessing, model training, and prediction (Random Forest, etc.)

Power BI – Data visualization and dynamic dashboards

Dataset – Includes parameters like NDVI index, humidity, rainfall, soil health, and crop type

## 📂 Dataset Description

The Smart Farming Crop Yield Dataset – 2024 contains environmental and operational variables affecting yield across 500 farms in India, USA, and Africa.

Link for dataset on kaggle : https://www.kaggle.com/datasets/atharvasoundankar/smart-farming-sensor-data-for-yield-prediction
## 📌 Columns Description

| Column Name             | Description |
|-------------------------|-------------|
| **farm_id**             | Unique ID for each smart farm (e.g., FARM0001) |
| **region**              | Geographic region (e.g., North India, South USA) |
| **crop_type**           | Crop grown: Wheat, Rice, Maize, Cotton, Soybean |
| **soil_moisture_%**     | Soil moisture content in percentage |
| **soil_pH**             | Soil pH level (5.5–7.5 typical range) |
| **temperature_C**       | Average temperature during crop cycle (in °C) |
| **rainfall_mm**         | Total rainfall received in mm |
| **humidity_%**          | Average humidity level in percentage |
| **sunlight_hours**      | Average sunlight hours received per day |
| **irrigation_type**     | Type of irrigation: Drip, Sprinkler, Manual, None |
| **fertilizer_type**     | Fertilizer used: Organic, Inorganic, Mixed |
| **pesticide_usage_ml**  | Daily pesticide usage in milliliters |
| **sowing_date**         | Date when crop was sown |
| **harvest_date**        | Date when crop was harvested |
| **total_days**          | Crop growth duration (harvest - sowing) |
| **yield_kg_per_hectare**| 🌾 Target variable: Crop yield in kilograms per hectare |
| **sensor_id**           | ID of the IoT sensor reporting the data |
| **timestamp**           | Random in-cycle timestamp when the data snapshot was recorded |
| **latitude**            | Farm location latitude (10.0 - 35.0 range) |
| **longitude**           | Farm location longitude (70.0 - 90.0 range) |
| **NDVI_index**          | Normalized Difference Vegetation Index (0.3 - 0.9) |
| **crop_disease_status** | Crop disease status: None, Mild, Moderate, Severe |


#### Key features include:

Environmental – Temperature, rainfall, humidity, sunlight

Operational – Fertilizer type, pesticide usage, irrigation type

Geographical – Region, crop type

Target Variable – Crop yield (kg per hectare)


## 🧠 Machine Learning with RapidMiner

<img width="1919" height="1068" alt="RapidMiner workflow" src="https://github.com/user-attachments/assets/09a120d6-c3ad-4237-99f2-4c8aa62324ad" />

Algorithm: Random Forest Regression

Input Features: Temperature, rainfall, humidity, sunlight, fertilizer type, pesticide usage, crop type, irrigation type, NDVI.

Output: Predicted yield (kg per hectare)

Result: Very low deviation between predicted and actual yield – reliable for forecasting future planting cycles.

## 📊 Key Insights
### 🌱 Crop Performance
| Crop    | Farms | Total Yield (kg) | Peak Yield Months | Insight                                        |
| ------- | ----- | ---------------- | ----------------- | ---------------------------------------------- |
| Cotton  | 107   | 420,039.53       | June → May → July | Best yield in late spring to early summer.     |
| Maize   | 111   | 442,063.48       | June → May        | Optimize irrigation in late spring.            |
| Rice    | 82    | 319,486.76       | June → May → July | Pre-monsoon care boosts yield.                 |
| Soybean | 108   | 459,735.92       | June → May → July | Consistent performance across seasons.         |
| Wheat   | 92    | 375,137.78       | June → May → July | Narrow yield window—focus efforts in May–June. |

### 🌍 Regional Performance

Top Regions: Central USA & South India (~21.6% each of total yield)

Yield correlates with balanced rainfall and sunlight.

### 🌦 Environmental Factors

Highest Avg Temp: Central USA (24.68°C)

Most Rain & Sunlight: South USA & South India

### 💧 Irrigation & Humidity

Best Yield: Sprinkler & Manual irrigation

Observation: Drip irrigation is efficient but yields lower output for certain crops.

### 🧪 Fertilizer & Pesticide Use

Inorganic fertilizers give the highest yields, especially for maize & cotton.

Pesticide use peaks in April–May, aligning with high-yield months.

### 🌿 NDVI (Crop Health Index)

Highest NDVI: Soybean & Rice (0.62)

Strong correlation between NDVI and yield up to 0.8.

## 📷 Dashboard Previews

<img width="500" height="675" src="https://github.com/user-attachments/assets/0b94aa60-aff5-4abc-babd-1a1b2786a4ba" /> <img width="500" height="676" src="https://github.com/user-attachments/assets/1c26ef7a-8563-4afe-b62f-3fc2ad546820" />
<img width="500" height="677" src="https://github.com/user-attachments/assets/f47d1b3d-30b4-4832-8aea-848bba2a26c0" /> <img width="500" height="673" src="https://github.com/user-attachments/assets/03e8c3ed-7f19-4ec7-9717-cf0166cdcbec" />
## 📈 Model Performance

Algorithm: Random Forest Regression

Validation: Predicted vs Actual yield scatter plot shows strong alignment.

## 📌 Use Cases

Farmers – Optimize resource allocation for maximum yield.

Researchers – Study environmental impact on crop productivity.

Policymakers – Develop targeted agricultural support programs.

## 🚀 How to Run This Project

1. Clone Repository

git clone https://github.com/yourusername/smart-farming-yield-dashboard.git


2. Run Yield Prediction in RapidMiner

Import .rmp process file

Load dataset

Run the prediction model

3. Visualize in Power BI

Open .pbix dashboard file

Connect to prediction output data
