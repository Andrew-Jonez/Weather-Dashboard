# Weather-Dashboard

This is a weather dashboard application that fetches weather data from the OpenWeather API and saves it to an AWS S3 bucket.

## Project Structure

```
weather-dashboard
├── data/                    # Directory for storing data files
├── src/
│   ├── __init__.py          # Package initializer
│   └── weather_dashboard.py # Main application logic
├── tests/                   # Directory for test files
├── .env                     # Environment variables
├── .gitignore               # Git ignore file
├── README.md                # Documentation for the project
└── requirements.txt         # Dependencies for the project
```

## Setup Instructions

1. **Clone the repository**:
   ```sh
   git clone <repository-url>
   cd weather-dashboard
   ```

2. **Create a virtual environment** (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the required dependencies**:
   ```sh
   pip install -r requirements.txt
   ```

4. **Set up environment variables**:
   Create a `.env` file in the root directory and add the following variables:
   ```
   OPENWEATHER_API_KEY=<your_openweather_api_key>
   AWS_BUCKET_NAME=<your_aws_bucket_name>
   AWS_ACCESS_KEY_ID=<your_aws_access_key_id>
   AWS_SECRET_ACCESS_KEY=<your_aws_secret_access_key>
   ```

5. **Run the application**:
   ```sh
   python src/weather_dashboard.py
   ```

## Usage Guidelines

- The application fetches weather data for predefined cities and saves the data to an AWS S3 bucket.
- The weather data includes temperature, feels like temperature, humidity, and weather conditions.
