# Capstone-Fars
📘 FARS Chatbot – Setup & Run Guide

Welcome to the FARS Chatbot project.
This tool provides an interactive interface for querying, analyzing, and working with FARS (Fatality Analysis Reporting System) data using Databricks, a lightweight Python backend, and a modern React frontend.

This guide walks you through setting up environment variables, preparing the backend, and running the full application.

🚀 1. Databricks Setup

Before running the project, you must obtain the required Databricks connection values.

Log into your Databricks workspace and collect the following:

DATABRICKS_HOST=
DATABRICKS_HTTP_PATH=
DATABRICKS_TOKEN=
DATABRICKS_WAREHOUSE_ID=


You will need these to configure the backend.

📁 2. Create the config Folder and .env File

Inside the User Interface directory, create a folder named:

config


Inside that folder, create a file named:

.env
Open .env and paste the following, filling in your actual Databricks values:

DATABRICKS_HOST=your_host_here
DATABRICKS_HTTP_PATH=your_http_path_here
DATABRICKS_TOKEN=your_token_here
DATABRICKS_WAREHOUSE_ID=your_warehouse_id_here

🖥️ 3. Running the Backend
Step 1 — Navigate into the backend folder:
cd User Interface/backend


Step 2 — Start the backend server:
uvicorn main:app --reload


The backend will now be running (usually at):

http://127.0.0.1:8000

🌐 4. Running the Frontend
Step 1 — Navigate into the frontend folder:
cd User Interface/frontend

Step 2 — Install dependencies:
npm install

Step 3 — Start the React application:
npm start


The frontend will open automatically in your browser, typically at:

http://localhost:3000

🎯 5. Using the Application

Once both servers are running:

The frontend provides the chat interface

The backend connects to Databricks, processes queries, and returns responses

Your .env file ensures secure access to Databricks data

You now have a fully functioning FARS Chatbot environment.