# Premium Car Dealership Website

## Overview
The **Premium Car Dealership Website** is a Node.js-based web application designed to showcase a car dealership's offerings. It features a home page displaying the available cars, an about page, an API endpoint for JSON data, and a contact page. The application is styled with CSS and includes images served locally.

## Features
- **Home Page**:
  - Displays a list of featured cars with images, names, and prices.
- **About Us Page**:
  - Provides information about the dealership and its values.
- **API Endpoint**:
  - Returns a JSON response with details of available cars.
- **Contact Page**:
  - Lists the dealership's contact information, including email, phone number, and address.
- **404 Page**:
  - User-friendly error page for non-existent routes.

## Prerequisites
- **Node.js** (v18 or higher)
- **npm** (comes with Node.js)
- **Docker** (if using Docker to deploy)

## Installation and Setup

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. **Install Dependencies**:
   ```bash
   npm install
   ```

3. **Set Up Local Images**:
   - Create a `public/images` directory inside the project folder.
   - Place car images in this directory and name them `car1.jpg`, `car2.jpg`, and `car3.jpg`.

4. **Run the Application**:
   ```bash
   node server.js
   ```

5. **Access the Website**:
   - Open your browser and navigate to `http://localhost:3000`.

## Docker Deployment

1. **Build and Run Using Docker Compose**:
   Ensure you have a `Dockerfile` and `docker-compose.yml` in the project root.

   ```bash
   docker-compose up --build
   ```

2. **Access the Application**:
   - Open your browser and navigate to `http://localhost:3000`.

3. **Stop the Application**:
   ```bash
   docker-compose down
   ```

## API Endpoint
- **URL**: `http://localhost:3000/api`
- **Response**:
  ```json
  {
    "message": "Welcome to our Car Dealership API!",
    "availableCars": [
      { "name": "2025 Sports Car", "price": "$50,000" },
      { "name": "2025 SUV", "price": "$40,000" },
      { "name": "2025 Sedan", "price": "$30,000" }
    ],
    "timestamp": "2025-01-19T00:00:00.000Z"
  }
  ```

## Directory Structure
```
project-root/
├── public/
│   └── images/
│       ├── car1.jpg
│       ├── car2.jpg
│       ├── car3.jpg
├── server.js
├── package.json
├── package-lock.json
├── Dockerfile
├── docker-compose.yml
```

## Customization
- **Add New Cars**:
  - Place new car images in the `public/images` folder.
  - Update the `/` route in `server.js` to include new car details.
- **Update Styling**:
  - Modify the CSS styles in the inline `<style>` blocks within the HTML responses.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

