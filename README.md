# Assessment: Data Representation Project

by Sarah McNelis - G00398343

<br>

## Introduction

This repository contains my project work for Data Representation as part of my Higher Diploma in Computing in Data Analytics. The objective of this project is to write a program that creates and consumes RESTful APIs. This involves creating a web application in Flask which has a RESTful API. This application should also link to a database table. And there should also be webpages which consume the API by performing CRUD operations. 

I have created a web application in Flask which links to two database tables and uses a RESTful API which is consumed by html webpages using AJAX calls to perfrom CRUD operations. 

<br>
 
## Setup

### Install the following

1. Download and install [anaconda](https://docs.anaconda.com/anaconda/install/index.html).
2. Download and install [cmder](https://cmder.app/).
3. Download and install [notepad++](https://notepad-plus-plus.org/downloads/)
4. Download and install [wampserver](https://www.wampserver.com/en/)

### Requirements text file

`requirements.txt` contains a list of all the packages requried to successfully run my flask server and it's RESTful API. 

### Running a python file

1. Open the command line at the appropriate respository. 
2. Type `python ` followed by the filename you wish to execute. 
3. The file will run. 

### Running a html file

1. Open the desired file in Notepad++
2. Click View on the toolbar
3. And click View Current File in and choose your preferred browser. 

### Accessing MySQL database and tables

1. Open wampserver
2. Click on MySQL and then on MySQL console
3. Enter username and password
4. Once the console is open type `SHOW DATABASES;`
5. For this I have named my database "project". So to acces the database type `USE project;`
6. To access the database tables `SHOW TABLES;`. This shows all tables available within that database. See image below of the current tables in my project database.  


![show_table](images/show_tables.jpg)


7. To see the arrivals table type `SELECT * FROM arrivals;`


![arrivals_table](images/arrivals.jpg)


8. To see the departures table type `SELECT * FROM departures;`


![departures_table](images/departures.jpg)


9. These tables can be accessed and updated using SQL commands from my python scripts. See `airportDAO.py` and execute in the command line. 


<br>


## Hosting the server

I have chosen to host my server on [pythonanywhere.com](https://www.pythonanywhere.com/). This is a good, user-friendly hosting service for python websites. 


If you would like to view my server arrivals and departures on pythonanywhere.com please click on the following links:

[Arrivals](http://sarahmcn25.pythonanywhere.com/arrivals)

[Departures](http://sarahmcn25.pythonanywhere.com/departures)

<br>

## What to expect
This repository contains:

- `homepage.html` - this document creates a fictional homepage for Shannon Airport where the user can select to view arrivals or departures. 

<br>

![homepage](images/homepage.jpg)

<br>

- `arrivals.html` - where I created a webpage based on fictional Shannon Airport arrival information. In this document you will find CRUD operations in the script section which allow the webpage to consume the API. For example, GET, POST, PUT and DELETE. The arrivals table is populated with data using AJAX calls to perform the GET operation. Similarily, if you click on the Create Arrvials button, you are making an AJAX call to POST data to the server. There is also functionality to Update and Delete arrivals using AJAX calls to perform the PUT and DELETE operations respectively. 

<br>

![arrivals](images/arrivalsPage.jpg)

<br>

- `departures.html` - where I created a webpage based on fictional Shannon Airport departure information. This also contains CRUD operations in the script section which allow the webpage to consume the API. This page uses the same functionality as arrivals.html expect for departures data this time. AJAX calls are made to perform CRUD operations to populate departures in a table, to create, to update and delete departures. 

<br>

![departures](images/departuresPage.jpg)

<br>

<br>

![create/update](images/createUpdate.jpg)

<br>

- `rest_server.py` - which creates an application server that will implement a RESTful API using Flask. 


- `airportDAO.py` - this program creates two classes - one for arrivals and one for departures. These contain functions to implement SQL commands from a python script. These classes are imported into the rest_server.py and used to perform CRUD operations. 

<br>


## Credits

- For this project I heavely relied on my lecturer's notes. You can access his github repository [here](https://github.com/andrewbeattycourseware/datarepresentation).


<br>

## References

- https://docs.python-guide.org/dev/virtualenvs/
- https://flask.palletsprojects.com/en/latest/
- https://realpython.com/python-requests/
- https://requests.readthedocs.io/en/latest/
- https://docs.python.org/3/library/urllib.html
- https://realpython.com/flask-connexion-rest-api/
- https://getbootstrap.com/docs/3.4/css/ 
- https://dev.mysql.com/doc/connector-python/en/connector-python-examples.html
- https://dev.to/gyi2521/ajax---get-post-putand-delete--m9j
- https://www.w3schools.com/html/html_scripts.asp
- https://hackerthemes.com/bootstrap-cheatsheet/#navbar__bg-dark
- https://levelup.gitconnected.com/create-interactive-html-tables-populated-with-api-data-dd5c467b0851

<br>

## End