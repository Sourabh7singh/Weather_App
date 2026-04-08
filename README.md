# ⛅ Saurabh Weather Application

A premium, modern weather web application built using React. This application provides real-time weather data, a 3-day forecast, and a detailed hourly forecast with dynamic visuals. Recently overhauled to feature a stunning dark-twilight aesthetic alongside hardware-optimized glassmorphism panels.

## 🚀 Features

- **Current Weather Conditions**: Accurate real-time data including precise temperature, humidity, wind speed, UV index, and atmospheric pressure.
- **Location Auto-Detect**: Effortlessly fetches weather metrics based on the user's current GPS location.
- **Search Capabilities**: Find real-time weather information for any specific city or location across the globe.
- **Interactive Forecasts**: View the upcoming 3-day general weather trends alongside an interactive, horizontally-scrollable hourly forecast.
- **Premium Glassmorphism UI**: High-end styling featuring frosted glass panels layered over a dynamic, twilight-colored background. 
- **Highly Responsive**: Fully adapts to all screen sizes—from ultrawide desktop monitors down to mobile devices, swapping layouts dynamically.
- **Optimized for Rendering**: Built to eradicate rendering bottlenecks (e.g., Chrome scroll stuttering during backdrop-filter execution) by intelligently isolating scroll layouts to dedicated GPU composite layers.

## 🛠️ Tech Stack & Tools

- **Frontend**: React.js (v18)
- **Styling**: Vanilla CSS3 (Custom Grid/Flex architectures, CSS variables, Glassmorphism, Google *Outfit* font)
- **State Management**: React Context API (`useContext`)
- **API Backbone**: [WeatherAPI.com](https://www.weatherapi.com/) via native `fetch` requests
- **Components**: Functional Components with standard React hooks (`useState`, `useEffect`)

---

## 💻 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Ensure you have Node.js and npm installed on your device.
- [Node.js](https://nodejs.org/) (Version 14.x or higher)
- npm (Usually comes bundled with Node.js)

### Installation & Set-up

1. **Clone the repository** *(or download the zip)*:
   ```bash
   git clone https://github.com/Sourabh7singh/Weather-Application.git
   ```

2. **Navigate to the Project Directory**:
   ```bash
   cd Weather-Application
   ```

3. **Install Dependencies**:
   ```bash
   npm install
   ```
   *This command installs all the necessary packages listed within the `package.json` file including Jest libraries and Web Vitals.*

4. **Environment Variables**:
   In order to run this application utilizing the weather data APIs, you should have your API configured. The application looks for `REACT_APP_API_KEY` defined in a `.env` root file. Currently, there is an embedded fallback key for immediate testing, but configuring your own robust WeatherAPI key is recommended.

5. **Run the Development Server**:
   ```bash
   npm run start
   ```
   *The application will automatically open in your default browser at `http://localhost:3000` (or `3001` if port 3000 is occupied).*

---

## 🎨 UI/UX Highlights

- **GPU Acceleration**: Advanced Chromium bottlenecks were side-stepped utilizing specific `-webkit-` optimizations, `translateZ`, and explicit `will-change: transform` to allow for flawlessly smooth scrolling.
- **Zero-clutch layout**: Media query scaling guarantees text fields, temperature indicators, and weather SVGs won't overlap uncomfortably regardless of device restrictions.

## 🤝 Contribution

This was a practice project. If you wish to propose improvements:
1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/NewFeature`).
3. Commit your Changes (`git commit -m 'Added exciting NewFeature'`).
4. Push to the Branch (`git push origin feature/NewFeature`).
5. Open a Pull Request.

---

> *Designed and developed by Saurabh.*
