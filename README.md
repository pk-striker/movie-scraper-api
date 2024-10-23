```markdown
# Movie Scraper API

A simple Node.js API built with Express that scrapes movie data from [mp4moviez.camera](https://www.mp4moviez.camera). The API allows you to fetch a list of movies, movie details, and download links.

## Features

- Fetch all movies from the website.
- Get details of a specific movie by ID.
- Retrieve download links for a specific movie.

## Technologies Used

- **Node.js** - JavaScript runtime
- **Express** - Web framework for Node.js
- **Axios** - Promise-based HTTP client for making requests
- **Cheerio** - Fast, flexible, and lean implementation of core jQuery for the server
- **Path** - Built-in Node.js module for file and directory paths

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/pk-striker/movie-scraper-api.git
   cd movie-scraper-api
   ```

2. Install the dependencies:

   ```bash
   npm install express axios cheerio axios-cookiejar-support tough-cookie
   ```

## Usage

1. Start the server:

   ```bash
   node server.js
   ```

2. Access the API at `http://localhost:3000`.

### API Endpoints

- **GET `/api/movies`**
  - Returns a list of all movies.

- **GET `/api/movies/:id`**
  - Returns details of a specific movie by its ID.

- **GET `/api/download-links`**
  - Requires a query parameter `link`.
  - Returns download links for the specified movie URL.

## Example

To get all movies:
```bash
curl http://localhost:3000/api/movies
```

To get details of a specific movie:
```bash
curl http://localhost:3000/api/movies/0
```

To get download links:
```bash
curl "http://localhost:3000/api/download-links?link=https://example.com/movie"
```

## Contributing

Feel free to submit issues or pull requests for improvements!

## License

This project is open source and available under the [MIT License](LICENSE).
```
