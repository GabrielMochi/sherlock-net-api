# Sherlock Net API

An API powered by NestJS and the Sherlock Project for searching and identifying usernames across multiple online platforms.

## Features

- Search for usernames across various websites.
- Fast and efficient username lookups.
- RESTful API built with NestJS.
- Easy deployment and scalability.

## Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/yourusername/sherlock-net-api.git
   cd sherlock-web-api
   ```

2. Install dependencies:

   ```sh
   yarn install
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory and configure necessary values.

4. Start the development server:

   ```sh
   yarn start:dev
   ```

## API Usage

### Search for a Username

```http
GET /search/:username
```

#### Response Example

```json
{
  "username": "exampleUser",
  "results": [
    {
      "platform": "Twitter",
      "url": "https://twitter.com/exampleUser",
      "exists": true
    },
    {
      "platform": "Instagram",
      "url": "https://instagram.com/exampleUser",
      "exists": false
    }
  ]
}
```

## Deployment

For production, build the project and start the server:

```sh
yarn build
yarn start
```

## Contributing

Pull requests are welcome! Please open an issue first to discuss proposed changes.

## License

This project is licensed under the MIT License.
