AIR BNB  App Clone
This project is a basic recreation of key features from AirBnB. It provides a command-line interface (CLI) for object management, a system for data persistence, and a static website layout for displaying content.

Table of Contents
Introduction

Core Functionalities

Setup Instructions

How to Use

Project Structure

Contributions

Licensing

Introduction
The goal of this project is to simulate essential components of a property rental platform. It features:

An interactive command interface for handling instances

A simple storage engine to save data using JSON

Unit testing to validate code functionality

A front-end static site built with HTML and CSS

Core Functionalities
Interactive CLI: Add, view, update, and remove data entries

Persistence Layer: Save and retrieve data using JSON serialization

Testing: Includes unit tests to ensure functionality and stability

Static Interface: A basic web UI for presenting information

Setup Instructions
To install and run the application:

bash
Copy
Edit
git clone https://github.com/your-username/airbnb-clone.git  
cd airbnb-clone
How to Use
To start the command-line interface:

bash
Copy
Edit
./console.py
Supported commands:

create <ClassName> – Create a new object

show <ClassName> <id> – Display an object

destroy <ClassName> <id> – Remove an object

all [ClassName] – List all objects or filter by class

update <ClassName> <id> <attribute> <value> – Modify an object

Example Commands
text
Copy
Edit
(hbnb) create User  
(hbnb) show User <id>  
(hbnb) update User <id> email "user@example.com"  
(hbnb) all User  
(hbnb) destroy User <id>
Project Structure
pgsql
Copy
Edit
├── AUTHORS  
├── console.py  
├── file.json  
├── models/  
│   ├── __init__.py  
│   ├── amenity.py  
│   ├── base_model.py  
│   ├── city.py  
│   ├── engine/  
│   │   ├── __init__.py  
│   │   └── file_storage.py  
│   ├── place.py  
│   ├── review.py  
│   ├── state.py  
│   └── user.py  
├── README.md  
├── tests/  
│   ├── test_base_model.py  
│   ├── test_base_model_dict.py  
│   ├── test_models/  
│   │   ├── test_amenity.py  
│   │   ├── test_city.py  
│   │   ├── test_engine/  
│   │   │   ├── __init__.py  
│   │   │   └── test_file_storage.py  
│   │   ├── test_place.py  
│   │   ├── test_review.py  
│   │   ├── test_state.py  
│   │   └── test_user.py  
│   ├── test_save_reload_base_model.py  
│   └── test_save_reload_user.py  
└── web_static/  
    ├── 0-index.html  
    ├── 1-index.html  
    ├── 2-index.html  
    ├── 3-index.html  
    ├── 4-index.html  
    ├── 5-index.html  
    ├── 6-index.html  
    ├── 7-index.html  
    ├── 8-index.html  
    ├── images/  
    ├── README.md  
    └── styles/
