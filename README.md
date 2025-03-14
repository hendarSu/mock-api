# Mock Server

This project is a mock server built with Express.js to simulate API responses for development and testing purposes.

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)

### Installation

1. Clone the repository:
    ```sh
    git clone <repository-url>
    cd mock-server
    ```

2. Install the dependencies:
    ```sh
    npm install
    ```

### Running the Server

To start the server, run the following command:
```sh
npm start
```

For development with automatic restarts on file changes, use:
```sh
npm run dev
```

The server will run on `http://localhost:3000`.

## Adding Mock APIs

To add a new mock API endpoint, follow these steps:

1. Open the `index.js` file located at `/Users/abushanum/Documents/project/natada/mock-server/index.js`.
2. Add a new route to handle the desired endpoint. For example, to add a new GET endpoint:
    ```javascript
    app.get('/path/to/your/api', (req, res) => {
        const responseData = {
            // Your mock response data
        };
        res.json(responseData);
    });
    ```

3. Save the file and restart the server if necessary.

### Example

To add a new endpoint for `/api/example`, you would add the following code to `index.js`:
```javascript
app.get('/api/example', (req, res) => {
    const responseData = {
        "message": "This is a mock response"
    };
    res.json(responseData);
});
```

Save the file and restart the server to see the new endpoint in action.

## License

This project is licensed under the MIT License.
````

</file>

This `README.md` file provides instructions on how to set up, run, and add new mock API endpoints to the project.