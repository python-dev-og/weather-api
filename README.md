![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
![Pandas](https://img.shields.io/badge/pandas-%20-yellow.svg)
![Flask](https://img.shields.io/badge/flask-%20-blue.svg)
![API](https://img.shields.io/badge/API-%20-green.svg)

# Flask Temperature Data API

## Overview
This Flask application provides a simple web interface and API for accessing temperature data. 
It allows users to view temperature records based on station ID, date, and year through a user-friendly web page and a RESTful API.

## Features
- **Web Interface:** A home page displaying a list of weather stations.
- **API Endpoints:**
  - Retrieve temperature data for a specific station and date.
  - Get all temperature data for a specific station.
  - Access yearly temperature data for a specific station.

## Requirements
- Python 3
- Flask
- Pandas

## Installation
1. Clone the repository or download the source code.
2. Install required packages: `pip install flask pandas`.

## Usage
- Run the application: `python app.py`.
- Visit `http://localhost:5000` in your browser for the web interface.
- Access API endpoints:
  - Specific date: `/api/v1/<station>/<date>`
  - All data for a station: `/api/v1/<station>`
  - Yearly data: `/api/v1/yearly/<station>/<year>`

## Data Format
- The application expects a `stations.txt` file containing station IDs and names.
- Temperature data files named `TG_STAIDxxxxxx.txt` for each station.

## Configuration
- Place your data files in the `data_small` directory.
- Ensure the data files follow the expected format.

## API Response Format
- JSON format, including station ID, date, and temperature.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contributions
Contributions are welcome. Please fork the repository and submit a pull request.

## Disclaimer
This is a sample application and should not be used as-is in a production environment.

