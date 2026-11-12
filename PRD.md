# AirWatch: AQI Monitoring, Forecasting and Analysis System

# 1. Project Overview

AirWatch is an Air Quality Index (AQI) monitoring, forecasting, and analysis system designed to provide information about air pollution levels in different cities. The system will collect air quality data from external sources, maintain historical records, provide future AQI forecasts, and allow users to analyze and compare pollution levels across different locations.

The primary objective of this project is to provide a centralized platform where users can monitor air quality, understand historical pollution trends, and obtain advance information about expected air pollution levels.

The project will focus on monitoring major air pollutants, including PM2.5, PM10, carbon monoxide (CO), nitrogen dioxide (NO2), sulfur dioxide (SO2), and ozone (O3).

# 2. Problem Statement
Air pollution is a significant environmental and public health concern these days

AirWatch aims to provide a centralized system that collects, stores, and presents air quality information. It will allow users to monitor current conditions, examine historical records, receive pollution alerts, and view upcoming AQI forecasts.

# 3. Project Objectives

The main objectives of AirWatch are:

  * Provide air quality information for multiple cities and monitoring locations.

  * Monitor major air pollutants and their concentrations.

  *  Maintain historical air quality records for analysis.

  *  Provide AQI forecasts to help users anticipate future pollution levels.

  *  Allow comparisons of air quality between different cities.

  *  Identify locations experiencing unhealthy pollution levels.

  *  Evaluate the accuracy of previously generated AQI forecasts by comparing them with actual measurements.

# 4. Functional Requirements
 The system will provide the following functionalities:
4.1 Air Quality Monitoring

 The system will retrieve air quality measurements from external data sources for selected cities and monitoring locations.

 Users will be able to:

   * View the latest available AQI for a selected city.

   * View individual pollutant concentrations, including PM2.5 and PM10.

   * View the corresponding AQI category, such as Good, Moderate, or Unhealthy.

 4.2 Historical Air Quality Analysis

 The system will maintain historical air quality records, allowing users to examine pollution levels over different periods.

 4.3 AQI Forecasting

 The system will provide future AQI forecasts for selected cities to help users anticipate upcoming pollution conditions.
 To keep forecasting consistent and manageable, the system will follow a fixed forecasting schedule:

   * A forecast for a particular date will be generated and retrieved three days in advance.

   * Only one forecast will be maintained for each city and target date.

For example, the forecast for November 9 will be retrieved on November 6. Forecasts retrieved on November 7 and November 8 will not replace the original forecast for November 9.
The system will display the predicted AQI and its corresponding category for the target date.

4.4 Forecast Accuracy Analysis

The system will evaluate the accuracy of its forecasts by comparing predicted AQI values with actual AQI measurements recorded for the same date.


4.5 City Comparison
Users will be able to compare air quality between multiple cities.

4.6 Pollution Alerts
NOTE: This is a feature that we have in mind but we are not committing to implement it. We will most probably implement it but if it becomes too complicated then we might have to abandon it.
The system will allow users to define pollution thresholds for a selected city .

For example, a user may configure an alert for when the AQI exceeds 150.
The system will identify measurements that violate these conditions and maintain corresponding alert records for users to view.

# 5. Scope of the Project
Scope has been defined above by functionalities that the system will provide 

6. Limitations and Exclusions
The system will not:

  * Develop its own algorithm to predict AQI.

  * Guarantee continuous real-time monitoring. Data availability and update frequency will depend on API providers.
  
  * Generate multiple revised forecasts for the same city and target date.

  * Send SMS messages, phone notifications, or automated emails.

  * Provide worldwide air quality coverage.

  
  * AQI forecasts and measurements will be obtained from available external data sources.

7. Expected Outcome
The expected outcome is a functional AQI monitoring and analysis platform that provides users with access to current and historical air quality information, future AQI forecasts, and pollution alerts.

The system will also provide analytical capabilities that allow users to compare pollution levels across cities and evaluate forecast accuracy.

This version keeps the focus on what AirWatch will achieve and what users will be able to do, without going into database schemas, SQL implementation, or technical architecture. It should fit approximately 2–3 pages with normal document formatting.
