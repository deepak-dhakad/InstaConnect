# InstaConnect
This project is a Social Media Recommendation System that scrapes data of users using Rapid API and stores it in MongoDB. The system then processes this data to create recommendations based on common followers and followings. The backend is implemented using Node.js and Express.

## Table of Contents
Features
Prerequisites
Installation
Usage
API Endpoints
Project Structure
Contributing
License
## Features
**Data Scraping:** Scrapes user data using Rapid API.
**Data Storage:** Stores scraped data in MongoDB.
**Data Processing:** Flattens nested data structures for easier processing.
**Recommendation System:** Generates recommendations based on common followers and followings.
**Search Functionality:** Allows searching for users based on keywords in their bio.
## Prerequisites
Before you begin, ensure you have met the following requirements:

Node.js and npm installed on your machine./n
MongoDB installed and running locally or on a server.
Rapid API Key for accessing the required API endpoints.
## Installation
To install the project, follow these steps:

Clone the repository:


git clone https://github.com/deepak-dhakad/InstaConnect.git
cd InstaConnect
Install the dependencies:


npm install
Set up your MongoDB connection URI and Rapid API key:  


// In your code, replace the URI and API key with your own  
**const uri** = 'mongodb://localhost:27017/';  
**const rapidApiKey** = 'YOUR_RAPID_API_KEY';  
## Usage
To use the project, follow these steps:

Start the server:


npm start
The server will run on port 3000 by default. You can access the various API endpoints to interact with the recommendation system.

## API Endpoints
### Flatten Documents
Endpoint: /flatten  
Method: GET  
Description: Flattens nested user data and stores it in a new collection.  
### Common Followers
Endpoint: /common-followers  
Method: GET  
Description: Retrieves users with common followers.  
### Recommendations
Endpoint: /recommendations  
Method: GET  
Description: Provides user recommendations based on common followers and followings.  
### Search Users
Endpoint: /users/:keyword  
Method: GET  
Description: Searches for users based on a keyword in their bio.  
**Parameters:**
keyword: The keyword to search for in user bios.
## Project Structure

recommendation-system/
│
├── app.js               # Main application file
├── package.json         # Project metadata and dependencies
└── README.md            # Project documentation
