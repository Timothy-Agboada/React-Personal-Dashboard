## 🚀 30-Day Coding Challenge: Day 30

This project is the thirtieth and final entry in my 30-day coding challenge. The goal was to build a comprehensive "capstone" application that brings together all the skills learned throughout the challenge. This Personal Dashboard demonstrates proficiency in fetching data from multiple APIs, managing various pieces of state with different React hooks, persisting data to `localStorage`, and composing a complex UI from smaller, independent components.

### 📖 Project Overview

This is a modern and visually appealing personal dashboard that provides a quick, at-a-glance overview of useful information. The dashboard is composed of several widgets: a real-time clock, a current weather display, a cryptocurrency price tracker, and a persistent to-do list. Each widget is designed as a self-contained component that fetches and manages its own data, showcasing a scalable and organized approach to building React applications.

### ✨ Live Demo & Screenshot

Below is a screenshot of the application's interface.
![Jul-04-2025 21-21-16](https://github.com/user-attachments/assets/ecf9b9a7-27c5-43af-938b-ff71f9fa8e07)


### 🌟 Key Features

* **Multi-Widget Layout:** A clean, grid-based dashboard featuring four distinct widgets:
    * **Live Clock:** Displays the current time and date, updating every second.
    * **Weather:** Fetches and displays the current weather for a predefined city.
    * **Crypto Prices:** Fetches and displays the current prices for Bitcoin, Ethereum, and Dogecoin.
    * **To-Do List:** A full CRUD to-do list that persists its data in `localStorage`.
* **Multiple API Integrations:** Fetches data in parallel from two different external APIs (OpenWeatherMap and CoinGecko).
* **Persistent State:** The to-do list saves its state to `localStorage`, so tasks are not lost on page reload.
* **Component-Based Architecture:** The application is highly modular, with each widget encapsulated in its own React component.
* **Asynchronous Data Fetching:** Each data-driven widget handles its own loading state and API calls using the `useEffect` hook.
* **Modern & Responsive UI:** A sleek dark theme with vibrant gradient backgrounds for each widget, styled with Tailwind CSS to be fully responsive.

### 💻 Technologies Used

This project was built using a modern, lightweight React setup.

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Babel](https://img.shields.io/badge/Babel-%23F9DC3e.svg?style=for-the-badge&logo=babel&logoColor=black)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)

* **React:** The core library for building the user interface and managing state.
* **ReactDOM:** Used to render the React component into the browser's DOM.
* **Babel:** Used as a transpiler to convert JSX into standard JavaScript.
* **Tailwind CSS:** For all styling and layout.
* **OpenWeatherMap API & CoinGecko API:** The sources for external data.
* **Font Awesome:** For icons.

### 🛠️ How to Run Locally

This project requires an API key from OpenWeatherMap to function fully.

1.  **Get a free API Key** from [OpenWeatherMap](https://openweathermap.org/).
2.  **Clone the repository (or download the code):**
    ```bash
    git clone https://github.com/timothy-agboada/react-personal-dashboard.git
    ```
3.  **Navigate to the project directory:**
    ```bash
    cd react-personal-dashboard
    ```
4.  **Add your API Key:**
    * Open the `index.html` file.
    * Inside the `<script type="text/babel">` tag, find the line `const WEATHER_API_KEY = 'YOUR_API_KEY';`
    * Replace `'YOUR_API_KEY'` with your actual key. You can also change the `WEATHER_CITY`.
5.  **Open the `index.html` file in your web browser.** The CDN links will handle loading all necessary libraries automatically.

### 🎯 Learning Objectives

This capstone project was a comprehensive application of all the concepts learned throughout the challenge:

* **Composing Complex UIs:** Building a sophisticated application by combining multiple independent, stateful components.
* **Managing Multiple Side Effects:** Using `useEffect` for various purposes in a single application: fetching data from multiple sources, setting up intervals, and interacting with `localStorage`.
* **Real-World Application Structure:** Simulating the structure of a real-world dashboard where different parts of the UI are responsible for their own data.
* **Combining Different State Types:** Managing local component state, persisted state (`localStorage`), and remote state from APIs all within one application.
