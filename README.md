# AirBnB Clone - Web Dynamic
![Project Architechture](https://s3.amazonaws.com/intranet-projects-files/concepts/74/hbnb_step5.png)

## Table of Contents
1. [Introduction](#introduction)
2. [Project Overview](#project-overview)
3. [Technologies Used](#technologies-used)
4. [Front-end](#front-end)
    - [HTML5](#html5)
    - [CSS](#css)
    - [JavaScript](#javascript)
5. [Back-end](#back-end)
    - [Python Flask Framework](#python-flask-framework)
    - [Restful API](#restful-api)
6. [Database](#database)
    - [MySQL](#mysql)
    - [SQLAlchemy ORM](#sqlalchemy-orm)
7. [Server Configuration](#server-configuration)
    - [Ubuntu 20.04 LTS](#ubuntu-2004-lts)
    - [Nginx](#nginx)
    - [HAproxy (Load Balancer)](#haproxy-load-balancer)
8. [Monitoring](#monitoring)
    - [Datadog](#datadog)
9. [Installation and Setup](#installation-and-setup)
10. [Project Structure](#project-structure)
11. [Bugs](#bugs)
12. [Authors](#authors)
13. [License](#license)

## Introduction
This project is a clone of the AirBnB platform, built to demonstrate a full-stack web application using modern technologies. The project includes a front-end developed with HTML5, CSS, and JavaScript, a back-end using the Python Flask framework, and a MySQL database managed through SQLAlchemy ORM. The application is deployed on an Ubuntu server, with Nginx and HAproxy for load balancing, and monitored using Datadog.

## Project Overview
The AirBnB Clone - Web Dynamic is the fourth segment of the AirBnB project at ALX / Holberton School that will collectively cover fundamental concepts of higher level programming. The goal of AirBnB project is to eventually deploy into our server a simple copy of the AirBnB Website.

## Technologies Used
- **Front-end:** HTML5, CSS, JavaScript
- **Back-end:** Python Flask framework, Restful API
- **Database:** MySQL
- **ORM:** SQLAlchemy ORM
- **Server:** Ubuntu 20.04 LTS, Nginx, HAproxy
- **Monitoring:** Datadog

## Front-end

### HTML5
HTML5 is used for structuring the web pages. It provides the semantic elements to create a well-organized document structure.

### CSS
CSS is used for styling the web pages, ensuring a responsive and visually appealing design across different devices and screen sizes.

### JavaScript
JavaScript is employed for dynamic interactions and client-side logic, enhancing the user experience through features like form validation, asynchronous requests, and interactive elements.

## Back-end

### Python Flask Framework
Flask is a lightweight WSGI web application framework in Python. It is used to build the back-end of the application, handling routing, templating, and serving static files.

### Restful API
The Restful API is designed to handle CRUD operations for different resources such as users, properties, bookings, and reviews. It follows REST principles, ensuring a stateless and scalable architecture.

## Database

### MySQL
MySQL is a relational database management system used to store and manage the application's data. It is chosen for its reliability, scalability, and ease of use.

### SQLAlchemy ORM
SQLAlchemy is an ORM for Python that provides a high-level abstraction for database interactions. It is used to map Python classes to database tables and manage database sessions.

## Server Configuration

### Ubuntu 20.04 LTS
Ubuntu 20.04 LTS is the operating system used for deploying the application. It is a popular choice for servers due to its stability, security, and support for a wide range of software.

### Nginx
Nginx is used as a web server and reverse proxy server. It is configured to serve static files, handle incoming requests, and forward them to the Flask application.

### HAproxy (Load Balancer)
HAproxy is used as a load balancer to distribute incoming traffic across multiple instances of the application, ensuring high availability and reliability.

## Monitoring

### Datadog
Datadog is a monitoring and analytics platform used to track the application's performance and health. It provides insights into server metrics, application logs, and error tracking.

## Installation and Setup
1. **Clone the repository:**
    ```sh
    git clone https://github.com/happychuks/AirBnB_clone_v4.git
    cd AirBnB_clone_v4
    ```

2. **Set up the virtual environment:**
    ```sh
    python3 -m venv venv
    source venv/bin/activate
    ```

3. **Install the dependencies:**
    ```sh
    pip3 install -r requirements.txt
    ```

4. **Configure the database:**
    - Install MySQL and create a database.
    - Update the database connection settings in the configuration file.

5. **Start the API:**
    ```sh
    python3 -m api.v1.app #API entry point
    #on another terminal run:
    curl -s -XGET http://0.0.0.0:5000/<pageName>/ 
    ```

6. **Start the application:**
    ```sh
    python3 -m web_dynamic.<pageName>
     #on another terminal run:
    curl -s -XGET http://0.0.0.0:5000/<pageName>/ 
    ```

7. **Set up Nginx and HAproxy:**
    - Configure Nginx to serve the application and handle static files.
    - Configure HAproxy to load balance the traffic.

8. **Set up Datadog:**
    - Install the Datadog agent on the server.
    - Configure the agent to monitor the application.

## Project Structure
```plaintext
AirBnB_clone_v4/
├── api
│   └── v1
│       └── views
│           └── documentation
├── models
│   └── engine
├── tests
│   └── test_models
│       └── test_engine
├── versions
├── web_dynamic
│   ├── static
│   │   ├── images
│   │   ├── scripts
│   │   └── styles
│   └── templates
├── web_flask
│   |
│   ├── static
│   │   ├── images
│   │   └── styles
│   └── templates
└── web_static
    ├── images
    └── styles
```

## Bugs

No known bugs at this time.

## Authors

AirBnb_clone_v4

- Happy Felix Chukwuma - [Github](https://github.com/happychuks) / [Twitter](https://twitter.com/Chukwuma__Happy) / [LinkedIn](https://www.linkedin.com/in/happyfelixchukwuma/)

AirBnb_clone_v3

- Happy Felix Chukwuma - [Github](https://github.com/happychuks) / [Twitter](https://twitter.com/Chukwuma__Happy) / [LinkedIn](https://www.linkedin.com/in/happyfelixchukwuma)
- Adioz Daniel - [Github](https://github.com/adiozdaniel)

Airbnb_clone_v2

- Happy Felix Chukwuma - [Github](https://github.com/happychuks) / [Twitter](https://twitter.com/Chukwuma__Happy)
- Temitope Alao - [Github](https://github.com/temmydhayor)

AirBnb_clone

- Happy Felix Chukwuma - [Github](https://github.com/happychuks) / [Twitter](https://twitter.com/Chukwuma__Happy)
- Adioz Daniel - [Github](https://github.com/adiozdaniel)

## License

Public Domain. No copy write protection.
