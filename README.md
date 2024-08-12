# Flight Search Web Application

This Flask-based web application allows users to search for flight availability across multiple partner programs. It features a simple, user-friendly interface for inputting search criteria and displays results dynamically.

## Features

- Search flights by origin, destination, and cabin class
- Supports multiple major airports including JFK, DEL, SYD, BOM, BNE, BLR, LHR, CDG, DOH, SIN
- Cabin options include Economy, Business, and First class
- Integrates with multiple airline partner programs:
  - Air Canada
  - United Airlines
  - KLM
  - Qantas
  - American Airlines
  - Etihad Airways
  - Alaska Airlines
  - Qatar Airways
  - LifeMiles
- Date range flexibility for departures (3 months window)
- Configurable number of stops (up to 2 stops)

## Installation

1. Clone this repository: git clone https:[//github.com/your-username/flight-search-app.git](https://github.com/namita9/FlightSearch/blob/main/FlightSearch/app.py)
2.  Navigate to the project directory: cd flight-search-app
3.  Install the required dependencies: pip install flask requests

## Usage

1. Run the application: python app.py
2. Open a web browser and go to `http://localhost:5000`
3. Use the search form to enter your criteria:
- Select an origin airport from the provided options
- Select a destination airport from the provided options
- Choose your preferred cabin class
- Click the "Search" button
4. The results will be displayed dynamically on the same page

## Project Structure

- `app.py`: The main Flask application file
- `templates/index.html`: The HTML template for the search interface
- `static/`: Directory for static files (CSS, JavaScript, etc.)

## API Integration

This application integrates with an external API to fetch flight data. The API endpoint used is `https://cardgpt.in/apitest`. The application sends a POST request with the following parameters:

- Origin and destination airports
- Cabin class
- Partner programs
- Number of stops
- Date range for departures

## Development

The application is set up with Flask's debug mode enabled, which allows for easy development and troubleshooting. To modify the search parameters or add new features, edit the `app.py` file.

### `app.py`

The main application file (`app.py`) contains the following key components:

- Flask application setup
- Route for the home page (`/`)
- Route for handling search requests (`/search`)
- Integration with the external API




### `index.html`

The HTML template (`index.html`) includes:

- A form for user input (origin, destination, cabin class)
    ![image](https://github.com/user-attachments/assets/73c263c3-245f-4df3-b91f-8b8f966a3aaf)
  
- A container for displaying search results
  
![image](https://github.com/user-attachments/assets/2c61b554-664a-4e0f-96c9-931aa79d9df5)

