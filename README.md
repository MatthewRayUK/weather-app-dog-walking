# Weather Forecast for Dog Walks 🌦️🐕

This app was created to help me decide the best times to walk my dog based on the weather. Every morning, it checks the forecast for specific times throughout the day (9am, 12pm, 3pm, and 6pm) and sends a message to my Facebook telling me whether it's likely to rain or stay dry. That way, I can plan the perfect time for a walk without getting caught in the rain!

## Features

- 🐕 **Dog Walk Planning**: Helps me choose the best times to walk my dog based on the weather.
- 🌦️ **Weather Data**: Retrieves the weather forecast for specific times during the day.
- 🌧️ **Rain Alerts**: Sends a message if it’s expected to rain, so I know when to bring an umbrella for my walk.
- ☀️ **Dry Day Alerts**: Lets me know when it’s expected to be dry, perfect for a walk without rain.
- 📅 **Daily Forecast**: Updates for 9am, 12pm, 3pm, and 6pm.
- 🖥️ **Facebook Integration**: Sends the forecast directly to my Facebook Messenger account for easy access.
- 🐕 **Dog-Focused**: Designed specifically to help dog owners plan their walks based on the forecast.

## Tech Stack

- **Backend**: Python
- **Weather Data**: OpenWeatherMap API
- **Facebook Integration**: Facebook API (requires environment variables)
- **Date and Time Handling**: `datetime` module for managing and formatting dates

## Installation

### Prerequisites

1. Set up a Facebook account and create an app on the [Facebook Developer platform](https://developers.facebook.com/) to generate a token.
2. Create an OpenWeatherMap account and get an API key for weather data.
3. Store your **Facebook token** and **OpenWeatherMap API key** as environment variables:
   - `FACEBOOK` = Your Facebook app token
   - `PARAM` = Weather API parameters (city, units, etc.)


### Example Output

Each morning, the app will send a message to my Facebook with the weather forecast, like this:

**If it will rain**:
```
🏞️🌦️Weather Forecast🌦️🏞️ 26/01/2025

☔ It will rain today, you will need an umbrella! ☔

9am: ☔ 
12pm: ☀️ 
3pm: ☀️ 
6pm: ☔
```

**If it will be dry**:
```
🏞️🌦️Weather Forecast🌦️🏞️ 26/01/2025

☀️ It will be a dry day! ☀️
```

9am: ☀️ 
12pm: ☀️ 
3pm: ☀️ 
6pm: ☀️
