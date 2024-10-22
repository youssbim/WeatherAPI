
# Weather Data API

A Flask application to provide weather data from various stations. 

## Setup
1. Make sure you have Python installed.
2. Install the required packages:
   ```
   pip install flask pandas
   ```
3. Place the data files in the `data_small` folder as per the expected naming convention.

## Running the Application
```
python app.py
```
The application will run at `http://127.0.0.1:5001`.

## API Endpoints

### 1. Home
- **URL:** `/`
- **Method:** GET
- **Description:** Displays a table of available stations.

### 2. Single Station, Single Date
- **URL:** `/api/v1/<station>/<date>`
- **Method:** GET
- **Example:** `/api/v1/2/2009-12-16`
- **Description:** Fetches temperature data for a specific station and date.

### 3. All Data for a Station
- **URL:** `/api/v1/<station>`
- **Method:** GET
- **Example:** `/api/v1/2`
- **Description:** Returns all temperature data for a specific station.

### 4. Yearly Data for a Station
- **URL:** `/api/v1/yearly/<station>/<year>`
- **Method:** GET
- **Example:** `/api/v1/yearly/10/2003`
- **Description:** Returns all temperature data for a specific station and year.
