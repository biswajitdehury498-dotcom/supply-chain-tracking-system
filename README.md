Supply Chain Tracking System

Project Overview

This Python-based system models and tracks the movement of shipments across various stages of a supply chain. It's built using Object-Oriented Programming (OOP) principles to manage individual units, track their historical status changes, and generate detailed reports.

Core Functionality & Features

Shipment Management: Each shipment is assigned a unique ID, tracks its current status, and maintains a full history of updates.

Centralized Tracking: The Tracker class handles the comprehensive management of all active and delivered shipments.

Menu-Driven Interface: The main.py entry point provides an easy-to-use console menu for all interactions.

ID Generation: Dedicated utility functions handle the creation of unique, traceable IDs.

Error Handling: Implements custom exceptions to ensure robust and user-friendly error management.

Project Structure

The codebase is organized into modular files for clear separation of concerns:

supply_chain_tracking/
│
├── main.py               # Entry point (menu-driven program)
├── shipment.py           # Defines the Shipment class (ID, status, history)
├── tracker.py            # Defines the Tracker class (manages all shipments)
├── report.py             # Reporting and history generation logic
├── exceptions.py         # Custom exceptions for error handling
├── utils.py              # Helper utilities (ID generation, timestamps)
│
├── data/                 
│   └── sample_data.json  # Optional dataset for persistence
│
└── README.md             # Project documentation (this file)

Learning Goals

This project is an excellent exercise in practical Python programming and OOP design:

OOP Mastery: Applying core concepts like encapsulation, classes (Shipment, Tracker), and composition.

History & State: Implementing mechanisms to track object state changes with timestamps.

I/O Operations: Practicing file handling for reporting and data persistence.

Exception Design: Creating and handling custom exceptions effectively.

Implementation Checklist (Tasks for Students)

The primary development tasks for this system are as follows:

Implement the Shipment class: Ensure it correctly handles ID, status, and the list of historical updates.

Implement the Tracker class: Build methods to manage the collection of shipments (add, retrieve, update).

Develop the User Menu: Create the menu in main.py to facilitate the main operations: Add Shipment, Update Status, View History, and Generate Reports.

Integrate utils.py: Use the helper functions for ID generation and possibly timestamping.

Implement Error Handling: Use custom exceptions from exceptions.py to handle errors gracefully (e.g., trying to update a non-existent shipment).

Extended Scope (Optional Challenges)

Data Validation: Implement validation in the Shipment class to only allow the following statuses: "Created", "Dispatched", "In Transit", "Delivered".

Data Persistence: Implement logic to Load and Save data in JSON format using the data/sample_data.json file.

Report Export: Implement the function in report.py to Export reports to a file (e.g., a .txt or .csv file).

