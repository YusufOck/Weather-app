# 🌦️ Mitawi Weather App (.NET MAUI)

![Mitawi Social Preview](https://raw.githubusercontent.com/danielmonettelli/dotnetmaui-mitawi-weather-app-challenge/main/Assets/Mitawi_GitHub_Social_Preview.png)

**Mitawi** is a cross-platform weather application developed using **.NET MAUI (Multi-platform App UI)**. It demonstrates a modern, clean UI/UX design and a robust **MVVM (Model-View-ViewModel)** architecture. The app provides real-time weather updates and detailed forecasts for locations worldwide using the OpenWeatherMap API.

This project serves as a comprehensive example of building production-grade apps with .NET MAUI, featuring custom handlers, converters, and responsive layouts for different device orientations.

## ✨ Features

* [cite_start]**Real-Time Weather Data:** Fetches current temperature, humidity, wind speed, and weather conditions[cite: 1204, 1226].
* [cite_start]**5-Day Forecast:** Provides a detailed weather prediction for the upcoming days[cite: 1226].
* [cite_start]**MVVM Architecture:** Implements a clean separation of concerns using Models, Views, and ViewModels[cite: 1986, 1987].
* [cite_start]**Responsive Design:** Includes specific layouts for Portrait and Landscape orientations (e.g., `HomePageOrientation.xaml`)[cite: 1984, 1967].
* [cite_start]**Platform Specifics:** tailored configurations for Android, iOS, MacCatalyst, Windows, and Tizen[cite: 1981, 1982].
* **Custom UI Components:**
    * [cite_start]Custom Font Icons using `CodeFontIcons`[cite: 1210].
    * [cite_start]SVG Image support[cite: 1248, 1982].
    * [cite_start]Custom Value Converters for data binding[cite: 1212, 1214].

## 📂 Project Structure

The solution is organized into the following key namespaces and folders:

* [cite_start]**`Mitawi/Models/`**: Contains data structures like `WeatherData.cs` that map the JSON responses from the API[cite: 1226, 1985].
* **`Mitawi/ViewModels/`**: Contains the business logic and state management.
    * [cite_start]`HomeViewModel.cs`: Manages the main dashboard data[cite: 1243].
    * [cite_start]`HomeDetailViewModel.cs`: Handles detailed weather views[cite: 1242].
    * [cite_start]`WelcomeViewModel.cs`: Logic for the onboarding screen[cite: 1244].
* **`Mitawi/Views/`**: The XAML UI pages.
    * [cite_start]`HomePage.xaml`: The main weather dashboard[cite: 1254].
    * [cite_start]`HomeDetailPage.xaml`: Detailed weather analysis page[cite: 1245].
    * [cite_start]`Orientations/`: Specific layouts for device rotation handling[cite: 1984].
* [cite_start]**`Mitawi/Services/`**: Contains `IWeatherDataService` and `WeatherDataService` for handling API network calls[cite: 1238, 1239, 1986].
* [cite_start]**`Mitawi/Converters/`**: Helper classes for XAML, such as `UnixTimeToDateTimeConverter` and `NegativeAndPositiveNumberConverter`[cite: 1214, 1217].
* [cite_start]**`Mitawi/Resources/`**: Contains Assets like `Fonts` (Roboto), `Images` (SVG), and `Styles`[cite: 1982, 1983].

## 🚀 Getting Started

To run this application, you need to configure the weather data provider using an **OpenWeatherMap API Key**.

### 🔑 Steps to Generate your API Key

1.  **Sign In:** Go to [openweathermap.org](https://openweathermap.org) and click on **Sign in**.
    ![OpenWeather Part1](https://raw.githubusercontent.com/danielmonettelli/dotnetmaui-mitawi-weather-app-challenge/main/Assets/OpenWeather_Part1.jpg)

2.  **Create Account:** Create your **Account** on OpenWeather if you don't have one.
    ![OpenWeather Part2](https://raw.githubusercontent.com/danielmonettelli/dotnetmaui-mitawi-weather-app-challenge/main/Assets/OpenWeather_Part2.jpg)

3.  **Navigate to API Keys:** Click on the **API Keys** tab in your dashboard.
    ![OpenWeather Part3](https://raw.githubusercontent.com/danielmonettelli/dotnetmaui-mitawi-weather-app-challenge/main/Assets/OpenWeather_Part3.jpg)

4.  **Generate Key:** Enter the **API key name** (e.g., "MitawiApp") and click **Generate**.
    ![OpenWeather Part4](https://raw.githubusercontent.com/danielmonettelli/dotnetmaui-mitawi-weather-app-challenge/main/Assets/OpenWeather_Part4.jpg)

5.  **Configure App:** * Open the solution in Visual Studio.
    * [cite_start]Navigate to `Mitawi/Constants/APIConstants.cs`[cite: 1211].
    * Paste your API key into the constant string variable.
    * Build and run the app!
    ![OpenWeather Part5](https://raw.githubusercontent.com/danielmonettelli/dotnetmaui-mitawi-weather-app-challenge/main/Assets/OpenWeather_Part5.jpg)

## 🛠️ Technologies Used

* **Framework:** [.NET MAUI](https://dotnet.microsoft.com/en-us/apps/maui)
* **Language:** C#
* **Markup:** XAML
* [cite_start]**Libraries:** * `CommunityToolkit.Mvvm` (for MVVM pattern support) [cite: 1211]
    * `Microsoft.Maui.Graphics` (for UI drawing)

## 📄 License

This project is licensed under the **MIT License**. [cite_start]See the [LICENSE](LICENSE) file for more details[cite: 1204].
