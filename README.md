# Marge: Python Weather App

Marge is a simple Python web application that provides current weather information for a specified city. It utilizes the Flask web framework and fetches data from the OpenWeatherMap API.

## Features

- Retrieve current weather data for any city.
- Display temperature, weather conditions, and "feels like" temperature.
- Simple and intuitive web interface.

## Prerequisites

- Python 3.x installed on your system.
- An API key from [OpenWeatherMap](https://openweathermap.org/api).

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Eosrebeldusky/Marge.git
   cd Marge
   ```

2. **Create a virtual environment:**

   ```bash
   python -m venv .venv
   ```

3. **Activate the virtual environment:**

   - On Windows:
     
     ```bash
     .venv\Scripts\activate
     ```
   
   - On macOS/Linux:
     
     ```bash
     source .venv/bin/activate
     ```

4. **Install the required dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

5. **Set up your OpenWeatherMap API key:**

   - Rename the `config_template.py` file to `config.py`:
     
     ```bash
     mv config_template.py config.py
     ```
   
   - Open `config.py` and replace `'YOUR_API_KEY'` with your actual OpenWeatherMap API key:
     
     ```python
     API_KEY = 'YOUR_API_KEY'
     ```

## Usage

1. **Run the application:**

   ```bash
   python server.py
   ```

2. **Access the application:**

   Open your web browser and navigate to `http://127.0.0.1:8000/`.

3. **Get weather information:**

   - Enter the name of the city in the search bar and submit.
   - The current weather details for the specified city will be displayed.

## Project Structure

```
Marge/
├── static/
│   └── styles/
│       └── style.css
├── templates/
│   ├── index.html
│   └── weather.html
├── .gitignore
├── config_template.py
├── requirements.txt
├── server.py
└── weather.py
```

- `server.py`: The main Flask application file that defines routes and handles requests.
- `weather.py`: Contains the function to fetch weather data from the OpenWeatherMap API.
- `templates/`: Directory containing HTML templates.
- `static/`: Directory containing static files like CSS.
- `config_template.py`: Template for configuration settings, including the API key.
- `requirements.txt`: Lists the Python dependencies for the project.

## Dependencies

- Flask
- Requests
- Waitress

These are specified in the `requirements.txt` file and can be installed using `pip`.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

*Note: Remember to keep your API key confidential and avoid sharing it publicly.*

