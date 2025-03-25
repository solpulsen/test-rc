# Power Outage Map - Recruitment Test Assignment

## Overview

Create a web application that displays power outages on a map in real-time. The application will consist of a .NET Web API backend that fetches outage data from an API endpoint and a React frontend that visualizes this data on an interactive map.

## Requirements

### Backend Requirements (.NET Web API)

1. Create a .NET Web API application that:
   * Fetches outage data from the provided API endpoint
   * Processes and serves the data to the frontend
   * Implements proper error handling
   * Provides appropriate API documentation (Swagger/OpenAPI)
   * Includes unit tests for critical functionality

2. API Endpoints to implement:
   * GET `/api/outages` - Returns all current outages
   * GET `/api/outages/{id}` - Returns details for a specific outage
   * GET `/api/outages/stats` - Returns statistics about outages (total affected customers, count by type, etc.)

3. Bonus:
   * Implement a background service that periodically refreshes the data
   * Set up a SignalR hub to push real-time updates to connected clients

### Frontend Requirements (React)

1. Create a React application that:
   * Displays outages on an interactive map (using libraries like Leaflet, Google Maps, or MapBox)
   * Shows outage details when a map marker is clicked
   * Provides basic statistics about current outages
   * Handles loading states and errors gracefully
   * Has a clean, responsive UI

2. Features to include:
   * Map visualization with markers/polygons for outages
   * Color-coding based on outage type (Planned vs Unplanned)
   * Simple dashboard showing summary statistics
   * Ability to filter outages (by status, type, etc.)

3. Bonus:
   * Implement real-time updates using SignalR
   * Add animations for new outages or status changes
   * Include a time-based visualization showing outage history

## Technical Requirements

### Backend
* ASP.NET Core 6.0 or newer
* Entity Framework Core (if using a database)
* RESTful API design
* Dependency Injection
* Appropriate error handling and logging
* Unit tests

### Frontend
* React (with hooks)
* TypeScript (preferred but optional)
* React Router for navigation
* A mapping library (Leaflet, Google Maps, or MapBox)
* CSS framework of your choice (or custom styling)
* Error boundary implementation

## Data Source
The backend should fetch data from the provided API endpoint. For testing purposes, you may use the provided JSON sample data as a mock.

## Evaluation Criteria
* **Functionality**: Does the application work as described?
* **Code quality**: Is the code well-structured, maintainable, and following best practices?
* **Error handling**: Does the application handle errors gracefully?
* **UI/UX**: Is the interface intuitive and user-friendly?
* **Documentation**: Is the code well-documented? Are there clear instructions for running the application?

## Submission Guidelines
1. Create a GitHub repository for your project
2. Include a README.md with:
   * Project overview
   * Setup instructions
   * API documentation
   * Any assumptions or design decisions you made
   * What you would improve with more time
3. Ensure the application can be set up and run with minimal effort

## Time Limit
This assignment is designed to be completed within 3 days, deadline is Friday 28th March, 23:59. Focus on delivering a working solution with clean code rather than implementing all bonus features.

Good luck!
