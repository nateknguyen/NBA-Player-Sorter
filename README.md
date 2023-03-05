# NBA-Player-Sorter

## Features
NBA-Player-Sorter is a web application built using Python, Flask, Bootstrap, and HTML/CSS.


NBA-Player-Sorter provides a simple user friendly interface to interact with NBA Player data that was sourced from the 1996-97 to 2020-21 NBA seasons. 

It allows the user to interact with the data in many different ways such as: searching by player names, draft round, or even seasons played.

Along with this, users have the option to add/delete/update players stored in the data base along with an algorithm to calculate a player's net rating with the ability to generate a visual representation of their net rating with a graph.

## Requirements
NBA-Player-Sorter requires `python3, flask, matplotlib, and mpld3` to be run.
## Installation
After following the instructions for installing Python3 from ```https://www.python.org/downloads/``` users will need to use the built in package installer for python `pip` to install the rest of the dependencies required for the application to run.

You can install these dependencies using the commands:
`pip3 install flask matplotlib mpld3`

After installing the dependencies, you will need to use the terminal to navigate to the folder containing the source code for this project where you will run: `python3 server.py` to start the server that can be accessed on your local machine.

Once done, the terminal will output an address you can input into your browser's address bar to access the application that is locally hosted on your machine.

## Functionality
`Search By Player Name` - allows the user to input any NBA player name that played within the span of the 1996-97 to 2020-21 NBA seasons and outputs their Name/Age/Draft Round/Points/Rebounds/Assists with the corresponding seasons

`Search By Draft Round` - allows the user to search for a specific draft round and outputs players that were drafted in that specified round. This even works with inputting "undrafted" to show all the undrafted players throughout the years

`Search By Season` - allows the user to specify a specific season they want to search for player data from

`Add Player` - allows the user to add a player who may be missing to the database by providing their Name and what Season they played

`Update Player` - allows the user to update the information of any existing player in the database with information such as: age, draft round, draft number, points, rebounds, and assists


`Delete Player` - allows the user to input the name and season played of any existing player and deletes them from the database. Do note that it will only delete a single season of the specified player not every occurrence of them in the database.

`Get Average Rating` - allows the user to input a specific season and draft round to calculate the average rating for that season's draft round which takes into account their statistics from that season including: points, rebounds, and assists with varied weighting for each category. This feature also allows a graph to be generated showing the user a visual representation of every single player's net rating compared to their draft number

`Calculate Player's Net Rating` - allows the user to input a player's name and calculate an average net rating over the entirety of their career in the NBA. This feature also includes a "generate graph" feature to create a bar graph showing the player's net rating compared to their age with specified min and max values
