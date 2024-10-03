# Weather Forecast App Using GetX

**Project Overview**  
Developed a real-time Weather Forecast app using Flutter and the OpenWeatherAPI, designed to provide users with current weather conditions, including temperature, humidity, wind speed, and location-based forecasts. This app incorporates best practices in state management using the GetX framework, allowing for efficient data handling and user interface updates. The app supports city search functionality, enabling users to view detailed weather updates for multiple locations, enhancing user experience and engagement.

### Features
- **Real-time Weather Updates**: Users can access up-to-date weather information sourced from the OpenWeatherAPI.
- **Location-Based Forecasts**: The app provides weather forecasts tailored to the user's selected cities.
- **City Search Functionality**: Users can search for and view weather updates for multiple cities seamlessly.
- **Efficient State Management**: Implemented GetX for optimal state management, making the app responsive and efficient.
- **Cross-Platform Compatibility**: The app is designed to work smoothly on both iOS and Android platforms.

### Tech Stack
- **Flutter**: A UI toolkit for building natively compiled applications for mobile, web, and desktop from a single codebase.
- **GetX**: A powerful and lightweight solution for state management, dependency injection, and route management.
- **OpenWeatherAPI**: An API that provides weather data for various locations worldwide.
- **JSON**: A format used for data exchange between the app and the OpenWeatherAPI.
- **HTTP**: A package used to make network requests to the API.

### Project Structure
Below is a breakdown of the key files in the project:

1. **`main.dart`**:
   - The entry point of the Flutter application. It sets up the app's initial routing and configuration, including the home page and dependency injection using GetX.

2. **`weather_controller.dart`**:
   - Contains the `WeatherController` class that extends `GetxController`. This file manages the state of the weather data, handles API requests to fetch weather information, and updates the UI based on the received data.

3. **`weather_model.dart`**:
   - Defines the `WeatherModel` class that represents the structure of the weather data retrieved from the OpenWeatherAPI. It includes attributes like temperature, humidity, and wind speed, and methods for parsing JSON data into model instances.

4. **`weather_service.dart`**:
   - This file contains the `WeatherService` class that is responsible for making HTTP requests to the OpenWeatherAPI. It handles the API key, constructs the request URLs, and processes the JSON responses to return weather data.

5. **`home_page.dart`**:
   - The main UI component of the app where users interact with the application. It displays the current weather conditions and allows users to search for different cities. The layout includes input fields, buttons, and sections to display weather information.

6. **`city_search.dart`**:
   - A widget that facilitates the search functionality for cities. It captures user input and triggers the search action, interacting with the `WeatherController` to fetch data for the specified city.

7. **`weather_details.dart`**:
   - A detailed view that displays comprehensive weather information for the selected city. It showcases the temperature, humidity, wind speed, and forecasts in a user-friendly layout.

8. **`styles.dart`**:
   - Contains style definitions and constants used throughout the app to maintain a consistent look and feel. This includes color schemes, text styles, and spacing.

9. **`assets/`**:
   - A directory containing image assets used in the application, such as weather icons and background images.

### Conclusion
This Weather Forecast app not only serves as a practical tool for users to stay updated on weather conditions but also demonstrates best practices in Flutter app development, including effective state management with GetX. The project showcases a robust architecture that can be expanded upon, making it an excellent foundation for future enhancements and features.
