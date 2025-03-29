# Weather App 🌦️

A modern weather application with real-time weather data, dynamic background themes, and intuitive UI. Built with React and OpenWeatherMap API.



## Tech Stack

- **Frontend**: 
  - React (with Hooks: useState, useEffect)
  - Tailwind CSS (for styling)
  - React Icons (for weather-related icons)
- **API**: 
  - OpenWeatherMap API (Weather Data & Geolocation)
- **State Management**: React Context API (for theme management)
- **Local Storage**: For persisting theme preferences
- **Build Tool**: Create-React-App

## Features

- Real-time weather information for any city worldwide
- Automatic location suggestions during search
- Temperature unit conversion (Celsius/Fahrenheit)
- Dynamic background themes based on weather conditions
- Dark/Light mode toggle
- Responsive design for all screen sizes
- Detailed weather metrics:
  - Humidity levels
  - Wind speed and direction
  - Visibility range
  - Sunrise/Sunset times
  - Feels-like temperature
  - Atmospheric pressure

## Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/weather-app.git
   cd weather-app

API Integration Details

OpenWeatherMap APIs Used

Current Weather Data
Endpoint: https://api.openweathermap.org/data/2.5/weather
Parameters: q={city}&appid={API_KEY}&units=metric
Returns: Current weather data including temperature, humidity, wind speed, etc.
Geocoding API
Endpoint: http://api.openweathermap.org/geo/1.0/direct
Parameters: q={query}&limit=5&appid={API_KEY}
Returns: Location suggestions based on partial city name input
Rate Limits

Free tier: 60 calls/minute
1,000,000 calls/month (with free account)
Consider adding request caching for production use

API key is stored in frontend code for development purposes only
For production deployment, consider:
Using environment variables
Implementing a backend proxy server
Enabling CORS restrictions in OpenWeatherMap account


Background animations change based on:
Day/Night cycle (using sunrise/sunset times)
Weather conditions (Clear, Clouds, Rain, etc.)
Theme preference is persisted using localStorage
Error handling includes:
Invalid city names
API rate limit warnings
Network errors
Responsive design ensures optimal viewing on:
Mobile devices (320px+)
Tablets (768px+)
Desktop (1024px+)

