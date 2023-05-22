# Flask F1 Race 

## App Overview

The Flask F1-Race application is a full stack web application built using Flask, SQLAlchemy ORM, and React. It enables users to view and edit F1 race-related data, including drivers, races, and driver-race statistics.

***

## Tech Stack
Python (3.8), Flask (Backend), SQLite3, SQLAlchemy (Database ORM), React (Frontend)

### Setup & Configuration
Backend Prerequisites: 

1.Python 3.8 
2.Pip

You can install the required libraries by running the following command in your terminal:

```$ pipenv install```

run the application: ```python app.py```

### Frontend
Prerequisites:

1.npm or yarn

### Steps
Open another terminal

1.cd client 
2.npm install (yarn install) 3.npm start

The application should now be running on ```localhost:3000```



## App Screenshots


### Homepage


![Homepage](client/src/assets/homepage.png)


## Drivers Page

***

The "DRIVERS" page show all drivers and their most basic info. Users have the option to "Ban" a driver, which deletes the driver from the front-end and the back-end database. A form to Add a new driver to the list is at the bottom of the page.

### Driver Model:

name: Driver's name represented as a string

car_number: Driver's car number represented as an integer

team: Driver's team represented as a string

driver_image: Url for the driver's image represented as a string

country: Driver's country represented as a string

podiums: Driver's podiums represented as an integer

dob: Driver's date of birth represented as an integer

bio: Driver's bio represented as a string

![Drivers Page](client/src/assets/driverspage.png)


### Drivers Details + Form


![Drivers Details + Form](client/src/assets/driversdet.png)


## Races Page

***

The "RACES" page shows a list of Circuits with their basic information. Similar to the Drivers page, this page has a form to Add a new race/circut to the list. You can also click on a specific track/circut to be taken to that specific circuit link and see more details about that race.

### Race Model

location: Race's location represented as a string

fastest_time: Fastest time recorded for this race represented as a float

track_image: Url for the Race's image represented as a string

track_length: Length of race represented as a float

first_event: Race's first event represented as a string

laps: Total laps for the race represented as an integer

details: Race details represented as a string

![Race Details + Form](client/src/assets/raceform.png)


## Race Stats

***


The "STATS" page shows a list of mock stats that show certain drivers' best lap time for a certain Race/Grand Prix. Users also have the ability to add driver stats with a form at the bottom of the page.


###DriverRace Model

driver_id: A foreign key representing the id of the driver assocaited with the join

race_id: A foreign keu representing the id of the race associated with the join

time: Driver's recorded time for the race represented as a float


![Race Stats](client/src/assets/racestats.png)