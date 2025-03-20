# Travel App Project

## Description
The Travel App is a web application that allows users to book trips by entering their destination and travel date. The app retrieves location details, weather forecasts, and relevant images using external APIs.


## Features
- User-friendly interface.
- Users can enter their destination and travel date into a form.
- Upon submission, the data is sent to the server for processing.
- The server interacts with three APIs to fetch:
- An image of the entered location.
- The weather forecast for the selected date.
- The retrieved information is displayed on the UI for the user.


## Installation
-Clone the repository:
git clone https://github.com/malakdaraghmeh/ProjectTrevel.git
cd travel_project


-Install dependencies: 
npm install

- Create a .env file in the root director:

Add the required API keys inside the .env file:
GEONAMES_USERNAME=your_geonames_username
PIXABAY_API_KEY=your_pixabay_api_key
WEATHERBIT_API_KEY=your_weatherbit_api_key

## Usage  

-Development Mode
Run the app in development mode:
npm run build-dev

-Production mode
  Run the app in production mode:
  npm run build-prod

-Running the server
  start the backend server:
  npm start

-Testing
  This project includes Jest tests for the form and the server.
  To run the tests:
  npm test

## Technologies
-Node.js v20.11.0

-Express.js for backend server

-Webpack for module bundling

-Axios for making API requests

-Jest for testing

-CSS & HTML for the frontend

## API Configuration
EndPoint:
POST /api

-Request body:
  {
  "location": "New York",
  "date": "2025-06-15"
  }

-Response:
  {
  "location": { "city": "New York", "country": "USA", "lat": 40.7128, "lng": -74.0060 },
  "weather": { "temp": 22, "description": "Clear sky", "date": "2025-06-15" },
  "image": "https://example.com/image.jpg",
  "countdown": 90
  }