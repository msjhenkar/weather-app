# weather-app
# Weather App

## Overview
The **Weather App** is a simple web application that allows users to check the current weather conditions for any city around the world. This project is built using **HTML**, **CSS**, and **JavaScript** and integrates with a weather API to fetch real-time data.

## Features
- Displays current weather information including temperature, humidity, wind speed, and weather conditions.
- Search functionality to get the weather for any city globally.
- Responsive design for an optimal viewing experience on different devices.
- Error handling for invalid city names or network issues.

## Technologies Used
- **HTML**: For structuring the web page.
- **CSS**: For styling the web application.
- **JavaScript**: For adding interactivity and making API requests.
- **Weather API**: The app uses the [OpenWeather API](https://openweathermap.org/api) to fetch real-time weather data.

## API Integration
The app integrates with the OpenWeather API to get weather data for different cities. The API provides the current temperature, weather description, and other useful information.

## Security considerations
Added api to config.js and is imported in script.js for security which is not visible in git repo

### How API Integration Works:
1. The user inputs the name of a city.
2. The app sends an HTTP GET request to the OpenWeather API with the city name.
3. The API responds with the current weather data for that city.
4. The weather information is displayed dynamically on the web page.

### Example API Request:
```javascript
const apiKey = 'YOUR_API_KEY';
const city = 'London';
const apiUrl = `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${apiKey}`;

