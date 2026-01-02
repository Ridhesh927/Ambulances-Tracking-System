# Ambulance Tracking System 🚑

A comprehensive, real-time solution designed to bridge the gap between emergency services and those in need. This project focuses on efficient ambulance dispatching and live location tracking to minimize response times during critical emergencies.

## 🚀 Key Features

*   **Real-Time Tracking**: Integration with **Leaflet.js** and **OpenStreetMap** to track ambulance movements LIVE on an interactive map.
*   **Intelligent Dispatching**: Implements a **Binary Search Tree (BST)** algorithm to efficiently sort and identify the nearest available ambulance to a user's location based on GPS data.
*   **Emergency Booking**: One-click booking system for patients with automatic location detection using the browser's **Geolocation API**.
*   **Admin Dashboard**: A centralized interface for administrators to:
    *   Monitor all active ambulances in the fleet.
    *   Add or remove ambulances and assign drivers.
    *   Update status (Available/Busy) and view real-time coordinates.
    *   Access detailed **Location History** for every vehicle.
*   **Driver Integration**: Dedicated login for drivers to manage their availability and report their current location.
*   **Smart Geocoding**: Uses the **Nominatim API** for seamless reverse geocoding (converting coordinates to human-readable addresses).

## 🛠️ Tech Stack

*   **Frontend**: HTML5, CSS3, Vanilla JavaScript (ES6+).
*   **Maps & Geolocation**: Leaflet.js, OpenStreetMap API.
*   **Algorithms**: Binary Search Tree (BST) for optimized proximity sorting; Haversine Formula for distance calculation.
*   **Icons**: Font Awesome 5.
*   **Persistence**: `localStorage` implementation for demo state management.

## 📈 How it Works

1.  **Detection**: When a user opens the "Emergency Booking" page, the system captures their GPS coordinates.
2.  **Calculation**: It calculates the distance to all "Available" ambulances using the **Haversine Formula**.
3.  **BST Optimization**: Ambulances are inserted into a Binary Search Tree based on their distance. An in-order traversal displays the nearest ambulances to the user first.
4.  **Action**: Once a user books an ambulance, the status is updated to "Busy," and the admin is provided with the user's contact details and location for immediate dispatch.

## 🛠️ Setup & Local Usage

1.  Clone this repository to your local machine.
2.  Open `index.html` in any modern web browser.
3.  **Pro Tip**: Since the project uses `localStorage`, your added ambulances and status updates will be saved even if you refresh the page!

---
Developed by **Ridhesh Mahajan**
*Developed to enhance emergency response and save lives through technology.*
