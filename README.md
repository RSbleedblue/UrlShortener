# URL Shortener

This is a simple URL shortener application built with React for the frontend and Node.js for the backend.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The URL Shortener application allows users to input a long URL and receive a shortened version that redirects to the original URL. This project is built using React for the frontend and Node.js with Express for the backend. The shortened URLs are saved in a JSON file.

## Features

- Shorten a long URL to a short URL
- Retrieve the original URL from a shortened URL

## Installation

### Prerequisites

- Node.js and npm installed on your machine

### Backend Setup

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/url-shortener.git
    cd url-shortener
    ```

2. Navigate to the backend directory and install dependencies:
    ```sh
    cd backend
    npm install
    ```

3. Start the backend server:
    ```sh
    npm start
    ```

### Frontend Setup

1. Navigate to the frontend directory and install dependencies:
    ```sh
    cd ../frontend
    npm install
    ```

2. Start the frontend development server:
    ```sh
    npm start
    ```

## Usage

1. Open your browser and navigate to `http://localhost:3000`.
2. Enter a URL in the input field and click "Create" to generate a shortened URL.
3. Use the shortened URL to be redirected to the original URL.

## API Endpoints

### POST /api/shortenLink

- Description: Shorten a long URL.
- Request Body:
    ```json
    {
        "link": "http://example.com"
    }
    ```
- Response:
    ```json
    {
        "working": "localhost:10000/api/{shortLink}",
        "status": true
    }
    ```

### GET /api/:shortlink

- Description: Retrieve the original URL from a shortened URL.
- Response:
    ```json
    {
        "working": "http://example.com",
        "success": true
    }
    ```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
