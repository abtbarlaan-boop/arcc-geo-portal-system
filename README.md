# ARCC Geo-Portal

A Web-Based GIS Map Viewer for the Department of Agrarian Reform's Community Clusters Development Plans.

![ARCC Geo-Portal Preview](https://via.placeholder.com/800x400.png?text=ARCC+Geo-Portal+Preview) 
<img width="1067" height="578" alt="image" src="https://github.com/user-attachments/assets/e4ffe570-3cfe-4872-8cd0-00e0be3e2a6d" />


## 📖 About The Project

This capstone project, developed for the Bachelor of Science in Information Technology at Don Bosco Technical College, involves the creation of the **ARCC Geo-Portal**. This is a web-based, interactive Geographic Information System (GIS) map viewer designed for the Philippine **Department of Agrarian Reform (DAR)**.

The system addresses the challenge of DAR's reliance on outdated methods like printed maps and spreadsheets by providing a centralized digital platform. It visualizes spatial data and development plans for **Agrarian Reform Community Clusters (ARCs)**, enhancing transparency, planning, and monitoring for both the public and DAR personnel.

### 🎯 Key Objectives

*   To develop a web-based system for the public to view, monitor, and track development projects.
*   To create an interactive map displaying project locations, coverage, and status.
*   To centralize project-related information for accuracy and consistency.
*   To provide a secure admin dashboard for authorized DAR personnel to manage data (CRUD operations).

## ✨ Features

### Public User Features
*   **Interactive Map Viewer:** Explore ARC locations using zoom, pan, and layer toggles.
*   **Thematic Data Layers:** View data on soil properties (Organic Matter, Phosphorus, Potassium) and major crops (Rice, Coconut, Corn, Cacao).
*   **Project Information:** Access detailed information about each Agrarian Reform Community (ARC).
*   **Resource Pages:** Learn More, Data, and Contact pages for additional context and transparency.

### Admin Features (DAR Personnel)
*   **Role-Based Access Control (RBAC):** Secure login for Super Admins and DAR Admins.
*   **Data Management (CRUD):** Full capabilities to Create, Read, Update, and Delete ARC data and information.
*   **User Management:** Super Admins can approve or reject new admin registrations.
*   **Centralized Dashboard:** Manage all system content from a single, secure interface.

## 🛠️ Built With

This project was implemented using the following technologies and frameworks:

*   **Frontend:** HTML5, Tailwind CSS, JavaScript
*   **Backend:** Python, Flask
*   **Database:** PostgreSQL (with PostGIS for spatial data)
*   **Mapping Library:** Leaflet.js
*   **Version Control:** Git, GitHub
*   **IDE:** Visual Studio Code

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

*   Python 3.x
*   PostgreSQL (with PostGIS extension)
*   pip (Python package manager)

### Installation

1.  **Clone the repo**
    ```bash
    git clone https://github.com/your-username/arcc-geo-portal-system.git
    cd arcc-geo-portal-system
    ```

2.  **Create a Virtual Environment (Recommended)**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install Python Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up the Database**
    *   Create a new PostgreSQL database.
    *   Enable the PostGIS extension: `CREATE EXTENSION postgis;`
    *   Configure your database connection string in the `config.py` file.

5.  **Initialize the Database**
    *   Run the scripts to create the necessary tables as defined in the Entity-Relationship Diagram (ERD).

6.  **Run the Application**
    ```bash
    flask run
    ```
    The application will be available at `http://localhost:5000`.

## 📁 Project Structure

```bash
arcc-geo-portal-system/
├── app/
│   ├── __init__.py
│   ├── models.py          # Database models
│   ├── routes.py          # Flask routes
│   ├── static/            # CSS, JS, images
│   └── templates/         # HTML files
├── migrations/            # Database migration scripts
├── config.py              # Configuration settings
├── requirements.txt       # Project dependencies
└── README.md
