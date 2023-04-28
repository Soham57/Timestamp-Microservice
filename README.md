Timestamp Microservice
This is a simple web application that takes in a time parameter in different formats and returns a JSON object containing the corresponding Unix timestamp and UTC time. The application can be accessed via the endpoint /api/time.

Usage
To use the Timestamp Microservice, simply make a GET request to the /api/time endpoint with the time parameter in one of the following formats:

ISO 8601: yyyy-mm-dd or yyyy-mm-ddTHH:MM:ssZ
Unix timestamp (in seconds): num
If the time parameter is valid, the application will return a JSON object containing the Unix timestamp and the corresponding UTC time in the following format:

{
"unix": <unix time>,
"utc": <utc time>
}

If the time parameter is invalid, the application will return a JSON object with an error message in the following format:

{
"error": "Invalid Date"
}

Technologies Used
This application was built using Node.js and the Express.js framework.

Installation and Setup
To run the application locally, follow these steps:

Clone the repository to your local machine.
Run npm install to install the dependencies.
Run npm start to start the server.
Access the application at http://localhost:3000/api/<date>.
