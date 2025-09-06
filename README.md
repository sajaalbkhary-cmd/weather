
# Weather Clean Architecture App

A simple Flutter weather app to practice Clean Architecture, API integration, and state management (Provider).

## ✅ Features
- Search weather by city
- Show temperature (°C), condition icon, and description
- Loading & error states
- Saves last searched city (bonus)
- Clean Architecture: Domain / Data / Presentation

## 🧰 Tech
- Flutter
- Provider (state)
- http (API calls)
- OpenWeather API (https://openweathermap.org/)

## 🔑 Setup (Very Important)
1) Get a free API key from OpenWeather: https://home.openweathermap.org/api_keys
2) Open `lib/features/weather/data/datasources/weather_api_service.dart`
3) Replace `const String _apiKey = "YOUR_API_KEY_HERE";` with your key.

## ▶️ Run
```bash
flutter pub get
flutter run
```

## 🧱 Structure
```
lib/
 └── features/weather/
      ├── domain/
      │    ├── entities/weather.dart
      │    ├── repositories/i_weather_repository.dart
      │    └── usecases/get_weather_by_city.dart
      ├── data/
      │    ├── datasources/weather_api_service.dart
      │    ├── models/weather_model.dart
      │    └── repositories/weather_repository_impl.dart
      └── presentation/
           ├── pages/home_page.dart
           └── providers/weather_provider.dart
```
