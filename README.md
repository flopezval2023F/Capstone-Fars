📘 FARS Chatbot – Setup & Run Guide

Welcome to the FARS Chatbot project.
This tool provides an interactive interface for querying, analyzing, and working with FARS (Fatality Analysis Reporting System) data using Databricks, a lightweight Python backend, and a modern React frontend.

This guide walks you through configuring Databricks credentials, preparing the backend, and running the full application.

🚀 1. Databricks Setup

Before running the project, you must obtain the required Databricks connection values.

Log into your Databricks workspace and collect the following:

DATABRICKS_HOST=
DATABRICKS_HTTP_PATH=
DATABRICKS_TOKEN=
DATABRICKS_WAREHOUSE_ID=

📁 2. Create the config Folder and .env File

Inside the User Interface directory, create a folder named:

config


Inside that folder, create a file named:

.env


Your structure should look like this:

User Interface/
 └── config/
      └── .env


Open .env and paste the following, filling in your actual Databricks values:

DATABRICKS_HOST=your_host_here
DATABRICKS_HTTP_PATH=your_http_path_here
DATABRICKS_TOKEN=your_token_here
DATABRICKS_WAREHOUSE_ID=your_warehouse_id_here

🖥️ 3. Running the Backend
Step 1 — Navigate into the backend folder:
cd "User Interface/backend"

Step 2 — Install dependencies:
pip install -r requirements.txt

Step 3 — Start the backend server:
python app.py


The backend will start running 

🌐 4. Running the Frontend
Step 1 — Navigate into the frontend folder:
cd "User Interface/frontend"

Step 2 — Install dependencies:
npm install

Step 3 — Start the React application:
npm start


The frontend will open automatically in your browser

🎯 5. Using the Application

Once both servers are running:

The frontend provides the FARS Chatbot user interface

The backend connects to Databricks and processes queries

The .env file supplies secure access to Databricks resources

You now have a fully operational FARS Chatbot environment.