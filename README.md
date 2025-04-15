# Node.js Server Project

This repository contains a simple **Node.js server** that serves static files and handles various content types. It includes features like custom event logging and graceful handling of non-existing pages.

## Features
- Serves files (HTML, CSS, JavaScript, JSON, images, etc.)
- Custom **event logging** using the `events` module
- Graceful handling of 404 errors (serves a custom 404 page)
- Redirects for specific pages (e.g., `/old-page.html` to `/new-page.html`)
- Modularized code for better maintainability


## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/suniltechs/Node_Server_Project.git
   cd node_server_project
   ```

2.Install the required dependencies:
  ```
  npm install
  ```

## Usage
1. Start the server:
   ```
   node server.js
   ```
2. Open your browser and navigate to:
   ```
   http://localhost:3500
   ```
3. The server dynamically serves files based on the URL and handles content types appropriately.

## Environment Variables
- PORT: The server will run on the port specified in the PORT environment variable, or default to 3500.

## Event Logging
### This server uses a custom event logging system:

- Logs all incoming requests with the URL and method.
- Logs errors into errLog.txt with detailed error messages.

## Error Handling
- Returns a custom 404 page for non-existing routes.
- Redirects:
  - /old-page.html → /new-page.html
  - /www-page.html → /

## Dependencies
- Node.js
- fs (File System Module)
- events (Event Emitter)

## Contributing
- Feel free to submit issues or pull requests to contribute to the project!
   
