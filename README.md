# Real-Time Tracker Application

A real-time location tracking application built using Node.js, Express, EJS, Socket.io, and Leaflet. This application enables real-time updates on a map, allowing users to track and visualize locations as they move.

## Features

- **Real-Time Location Sharing**: Uses Socket.io to transmit location data instantly to all connected clients.
- **Interactive Map Visualization**: Leverages Leaflet to display real-time location updates on a map.
- **User Disconnection Handling**: Removes markers from the map when a user disconnects.
- **Responsive Map Display**: The map view is dynamically centered on new location data.

## Tech Stack

- **Node.js**: Server-side JavaScript runtime.
- **Express**: Web framework for Node.js, used to serve static files and handle routing.
- **EJS**: Templating engine for rendering dynamic HTML views.
- **Socket.io**: Library for real-time, bidirectional event-based communication.
- **Leaflet**: JavaScript library for mobile-friendly, interactive maps.

## Prerequisites

Make sure you have the following installed:

- **Node.js** (v12+)
- **npm** (Node Package Manager)

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/realtime_tracker.git

2. **Navigate to the project directory**:
   cd realtime_tracker

3. **Install dependencies**:
   npm install


## Usage
1. **Start the server**:
    npm start


The application will run on http://localhost:4000 by default.

Access the Application: Open your browser and go to http://localhost:4000 to view the real-time tracker.

Enable Location Sharing: When prompted, allow location sharing in your browser to send location data to the server.


## Functionalities
**Real-Time Location Updates**: Uses Geolocation API to send location updates and broadcast them to all connected clients.
**Map Visualization**: Displays users' real-time location on an interactive Leaflet map.
**Dynamic Marker Management**: Adds markers for new users and removes them when a user disconnects.
**Automatic Map Centering**: Centers the map on the latest location update.


## How It Works
**Backend**:
app.js sets up an Express server with Socket.io for real-time communication.
When a user connects, the server listens for location data sent by the client and broadcasts it to all clients.
On disconnection, the server notifies other clients to remove the disconnected user's marker.

**Frontend**:
index.ejs renders a basic HTML structure and includes client-side JavaScript.
public/script.js uses the Geolocation API to track the user’s location and send it to the server.
Leaflet displays the location on an interactive map, creating a marker for each user and updating or removing it as needed.

## Dependencies
**express** - Fast, minimalist web framework for Node.js
**ejs** - Templating engine for generating dynamic HTML
**socket.io** - Enables real-time, bidirectional event-based communication
**leaflet** - JavaScript library for interactive maps



   
