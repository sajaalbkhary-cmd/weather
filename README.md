# weather
# Weather Clean Architecture App

A simple Flutter weather app to practice Clean Architecture, API integration, and state management (Provider).

## ✅ Features
- Search weather by city
- Show temperature (°C), condition icon, and description
- Loading & error states
- Saves last searched city (bonus)
- Clean Architecture: Domain / Data / Presentation

## 🧰 Tech Stack
- **Flutter** (SDK)
- **Provider** (State Management)
- **http** (API calls)
- **OpenWeatherMap API** (Data source)

## 📸 Screenshots

| Home Screen (Loading) | Weather Results | Error State |
| :-------------------: | :-------------: | :---------: |
| <img src="./screenshots/loading.png" width="200"> | <img src="./screenshots/result.png" width="200"> | <img src="./screenshots/error.png" width="200"> |

## 🔑 Setup (Very Important)

1.  **Get a free API key** from [OpenWeatherMap](https://home.openweathermap.org/api_keys). (It may take a few hours for the key to activate).
2.  **Clone the repository** and open it in your IDE.
    ```bash
    git clone https://github.com/your-username/weather-app.git
    cd weather-app
    ```
3.  **Add your API key:**
    - Open the file: `lib/features/weather/data/datasources/weather_api_service.dart`
    - Find the line: `const String _apiKey = "YOUR_API_KEY_HERE";`
    - **Replace `"YOUR_API_KEY_HERE"` with your actual key**, keeping the quotes.
    ```dart
    // Example after change
    const String _apiKey = "abc123def456ghi789jkl012";
    ```

## ▶️ How to Run

1.  **Get dependencies:**
    ```bash
    flutter pub get
    ```
2.  **Run the app on a connected device or emulator:**
    ```bash
    flutter run
    ```

## 🧱 Project Structure (Clean Architecture)
