JSON Parser and Viewer

This project is a simple web-based JSON parser and viewer built with JavaScript. It allows users to input JSON data via text or file upload and displays the data in a collapsible tree structure. The project helps visualize and interact with JSON objects, enabling easier understanding of complex, nested JSON data.
Features

    JSON Input: Users can paste JSON text directly into the input field or upload a JSON file.
    JSON Parsing: The inputted JSON is parsed into a JavaScript object using JSON.parse(). If the JSON is invalid, an error message is displayed.
    Collapsible Tree View: The parsed JSON is displayed as a tree structure. Objects and arrays can be collapsed and expanded to make it easier to explore nested data.
    Error Handling: If the input is not valid JSON, an error message in red is displayed.
    File Upload: Users can upload a .json file, and its content will be automatically parsed and displayed.

Project Structure
1. HTML

Contains the basic structure of the webpage, including:

    A text area for inputting JSON
    A file input for uploading JSON files
    A section to display the parsed and formatted JSON

2. JavaScript

Handles the parsing, tree generation, and user interactions:

    parseAndDisplayJson(): Retrieves JSON from user input or file, parses it, and triggers the tree-building function.
    buildTree(): Recursively builds a tree structure to represent the JSON data, adding collapsible features for nested objects and arrays.
    getType(): Determines the type of each JSON value (e.g., string, number, array, or object) for appropriate CSS styling.

3. CSS

Provides styles for:

    Formatting keys and values
    Adding collapsible functionality
    Displaying error messages for invalid JSON

Usage
  1. Input JSON via Text

    Paste your JSON string into the input field.
    Click the "Parse" button or trigger the parsing through your application.
    The parsed JSON will be displayed in a collapsible tree structure.

  2. Input JSON via File Upload

    Click on the "Choose File" button to select a .json file from your system.
    Once selected, the file content will be displayed and parsed automatically.

  3. Explore the JSON

    Expand or collapse objects and arrays by clicking on their keys to explore the structure of the JSON.

How to Run

    Clone or download this project to your local machine.
    Open the index.html file in any web browser.
    Input a JSON string or upload a JSON file to see the parsed output.


Example

    If the following JSON is inputted:

    json

    {
        "name": "John Doe",
        "age": 30,
        "address": {
            "city": "New York",
            "zip": "10001"
        },
        "phones": ["123-456-7890", "987-654-3210"]
    }

    The output will display a collapsible tree structure with name, age, address, and phones as keys. The address and phones sections can be expanded to show further nested data.

Error Handling

    If the JSON input is invalid, an error message saying Invalid JSON will be displayed in red.

Browser Compatibility
  
    The project works in all modern web browsers that support JavaScript and the FileReader API.
License

    This project is open-source and available under the MIT License.
