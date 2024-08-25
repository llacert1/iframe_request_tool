
# Iframe Request Tool

This project provides an interactive web interface for modifying and testing iFrame parameters. It is designed to help developers easily configure URL parameters, select different HTTP request methods, and test their impact within an embedded iFrame. The interface also allows users to save configurations to a file and load them back, providing a seamless way to manage testing scenarios.

## Features

- **Modify iFrame Parameters:**
  - Allows you to set a base URL and up to six parameters for the iFrame.
  - Each parameter can be named, assigned a value, and toggled on or off.
  - Parameters are automatically encoded and appended to the base URL when the "Update iFrame" button is clicked.

- **Select HTTP Request Method:**
  - Provides a dropdown menu to select the type of HTTP request to be sent to the URL.
  - Supported HTTP methods include `GET`, `POST`, `PUT`, `DELETE`, `PATCH`, `HEAD`, and `OPTIONS`.

- **Dynamic iFrame Update:**
  - Once parameters are set and the HTTP method is selected, the iFrame is dynamically updated to reflect the current URL with the specified parameters and method.

- **Request and Response Logging:**
  - The interface logs the URL sent to the iFrame along with the selected HTTP method and captures the response returned from the iFrame’s content.
  - Logs are displayed in a dedicated area below the iFrame.

- **Save and Load Configurations:**
  - You can save the current configuration (base URL, HTTP method, and parameters) to a JSON file on your workstation.
  - Load a previously saved configuration to quickly restore the iFrame settings.

- **Clear Functionality:**
  - A "Clear iFrame and Logs" button is available to reset the iFrame and clear all logs.

## How to Use

1. **Select HTTP Method:**
   - Choose the desired HTTP method from the dropdown menu (e.g., `GET`, `POST`, etc.).

2. **Set the Base URL:**
   - Enter the base URL in the input box labeled "Base URL."

3. **Configure Parameters:**
   - For each parameter (up to six), enter a name and value in the corresponding input fields.
   - Use the checkbox to enable or disable each parameter.

4. **Update iFrame:**
   - Click the "Update iFrame" button to apply the changes. The iFrame will reload with the new URL, including the configured parameters and selected HTTP method.
   - The request and response logs will update to reflect the new request.

5. **Save Configuration:**
   - Click the "Save to File" button to download the current configuration as a JSON file (`params.json`).

6. **Load Configuration:**
   - Click the "Upload File" button and select a JSON file to load a saved configuration. The form will auto-populate with the loaded data.

7. **Clear Logs and iFrame:**
   - Click the "Clear iFrame and Logs" button to reset the iFrame and clear the request and response logs.

## Project Structure

- **HTML File:**
  - The HTML file contains all the logic and UI for modifying the iFrame parameters, selecting the HTTP method, updating the iFrame, logging requests and responses, and handling file operations (save/load).

- **JavaScript Functions:**
  - `updateIframe()`: Updates the iFrame with the configured URL and logs the request and response.
  - `clearLogsAndIframe()`: Clears the iFrame and resets the logs.
  - `saveToFile()`: Saves the current base URL, HTTP method, and parameters to a JSON file.
  - `loadFromFile(event)`: Loads a configuration from a JSON file and updates the form fields.

## Requirements

- This project is a standalone HTML file and does not require any external dependencies.
- It runs in any modern web browser.

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute this software.
