# ASCII Art Web

ASCII Art Web is a simple web application that allows users to generate ASCII art based on different art styles and input text. Users can select an art style and provide text, and the application will generate and display ASCII art corresponding to the chosen style.

## Features

- Select from different art styles: Standard, Shadow, ThinkerToy.
- Input your own text to generate custom ASCII art.
- User-friendly web interface for easy interaction.


## How to Run
To run the application, follow these steps:
1. Clone the repository to your local machine.
```bash
https://github.com/Githaiga22/ascii-art-web.git
```
2. Navigate to the project directory in your terminal.
3. Run the application: 
```bash
go run main.go
```
4. Open a web browser and navigate to http://localhost:8080


## Implementation Details: Algorithm
The application uses the following algorithm to generate ASCII art:

1. The user inputs text and selects a banner using the GUI.
2. The application sends a POST request to the /ascii-art endpoint with the user's input.
3. The server processes the request and generates the ASCII art using the selected banner.
4. The server returns the generated ASCII art as an HTTP response.
5. The client-side JavaScript code receives the response and displays the ASCII art on the page.

## HTTP Endpoints
The application implements the following HTTP endpoints:

GET /: Returns the main page HTML response.
POST /ascii-art: Sends data to the server (text and banner) and returns the generated ASCII art as an HTTP response.

## HTTP Status Codes
The application returns the following HTTP status codes:

- 404 Not Found: Nothing is found (e.g., templates or banners).
- 400 Bad Request: Incorrect requests.
- 500 Internal Server Error: Unhandled errors.

## Notes
- The application uses Go templates to receive and display data from the server.
- The application uses form and other types of tags to make the POST request.
- The way the result from the POST is displayed is up to the developer's choice. Recommendations include displaying the result in the route /ascii-art after the POST is completed or appending the results in the home page.

## Usage

1. Open the web application in your browser.
2. Select an art style from the provided options.
3. Enter the text you want to convert to ASCII art.
4. Click the "Generate" button to see the generated ASCII art.

## Authors
-  Githaiga22

## Github Profile
- GitHub Profile: [Githaiga22](https://github.com/Githaiga22)
## Contributing

Contributions are welcome! If you find any issues or want to improve the application, feel free to submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
