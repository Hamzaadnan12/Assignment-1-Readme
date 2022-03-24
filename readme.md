<div id="top"></div>


<!-- ABOUT THE PROJECT -->
# About The Project

![Product Name Screen Shot][product-screenshot]

This is a CRUD web application using React, Flask, Python, JavaScript, HTML and CSS.

Structure of the application:
* A student contains a name and number of credits earned.
* A course contains a course title, and instructor
* An instructor contains a name, and course department
* There is a many-to-many relationship between a student and a course; in other words, a student can be enrolled in an unlimited number courses and a single course can have an unlimited number of students enrolled in it


<p align="right">(<a href="#top">back to top</a>)</p>



## Built With

This project was built with these frameworks and applications.


* [React.js](https://reactjs.org/)
* [Bootstrap](https://getbootstrap.com)
* [Node JS](https://nodejs.org/en/)
* [Flask](https://flask.palletsprojects.com/en/2.0.x/)
* [SQL Alchemy](https://www.sqlalchemy.org/)
* [XAMPP](https://www.apachefriends.org/download.html)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

Start by downloading and installing XAMPP, Python and Node JS.
* [XAMPP](https://www.apachefriends.org/download.html)
* [Python](https://www.python.org/downloads/)
* [Node JS](https://nodejs.org/en/) 

### Prerequisites

Make sure your Node is fully updated before running further npm commands.
* npm
  ```sh
  npm install npm@latest -g
  ```

## Flask Installation

_Make sure this project directory is placed into a resonable place and use the terminal to interact with the application and installation._

1. Download Python: https://www.python.org/downloads/
2. Install Flask
   ```sh
    pip install Flask
   ```
3. Install Marshmallow
   ```sh
    pip install flask-marshmallow
   ```
4. Install SQLAlchemy
    ```sh
    pip install Flask-SQLAlchemy
   ```
   ```sh
    pip install mysqlcleint
   ```
   ```sh
    pip install marshmallow-mysqlcleint
   ```



<p align="right">(<a href="#top">back to top</a>)</p>

## Set up SQL Alchemy and create database

_Make sure this project directory is placed into a resonable place and use the terminal to interact with the application and installation._

1. Open XAMP
2. Click on Start for Modules *Apache* and *MySQL*
    ![XAMPSTART][XAMP-start]
3. Open any web browser of your choice and open phpMyAdmin with the following link:
   ```sh
    http://localhost/phpmyadmin/
   ```
4. Click on new and create a new database called *flaskdb*
    ![dbCreate][create-db]
5. Open a new Terminal/Command Prompt and go into the *backend* directory of this project. Run the following commands:
    ![dbCommand][command-db]    
   ```sh
    python
   ```
   ```sh
    from app import db
   ```
   ```sh
    db.create_all()
   ```
## Activate Virtual Enviorment

_Make sure this project directory is placed into a resonable place and use the terminal to interact with the application and installation._

1. Open terminal or command prompt
2. Open the A1 directory and type in the following command:
#### For Windows, run:
   ```sh
    venv\Scripts\activate.bat
   ```
#### For Unix or MacOS Run:
  ```sh
    source venv\Scripts\activate
   ```
#### The terminal should look like this:
![venv activate][venv-activate]

<p align="right">(<a href="#top">back to top</a>)</p>

## Run Flask Application

_Make sure this project directory is placed into a resonable place and use the terminal to interact with the application and installation._

1. Open Terminal/Command Prompt
2. Activate virtual enviorment shown above
3. Open the *backend* directory and type the following command:

   ```sh
    python app.py
   ```
   ![flask][flask-run]
Do not close this terminal window.


## Run React Application

_Make sure this project directory is placed into a resonable place and use the terminal to interact with the application and installation._

1. Open a New Terminal/Command Prompt
2. Open the *frontend* directory and type the following command:

   ```sh
    npm start
   ```
Do not close this terminal window


<!-- USAGE EXAMPLES -->
# Usage

This CRUD Web Applications contains 4 Datatables:
1. Instructors
2. Students
3. Courses
4. Grades

We can Insert, Update, Delete in the Instructors, Students, and Courses table. But we cannot Update, but only Insert and Delete for the Grades data table. This is because the Grades table has a Many-to-Many relationship with Students and Courses.

## Insertion Demo
![insert-data][insert-data]
## Update Demo
![update-data][update-data]
## Delete Demo
![delete-data][delete-data]
## Insertion in the Courses Table
![insert-data][insert-data-courses]
## Insertion in the Grades Table
![insert-data][insert-data-grades]
### Matching Primary Keys from Grades Table
![primaru-key][primary-key]
#### We can see that each primary key from the Student and Course table is stored into our Grades table.


<p align="right">(<a href="#top">back to top</a>)</p>


## Credits

Owner/Creater: Hamza Adnan


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[product-screenshot]: (https://github.com/Hamzaadnan12/Assignment-1-Readme/blob/main/img/main.png)
[XAMP-Start]: img\XAMPstart.png
[create-db]: img\phpadmin-db-create.png
[command-db]: img\command-db.png
[venv-activate]: img\venv-activate.png
[flask-run]: img\flask-run.png
[primary-key]: img\primary-key-match.png
[insert-data]: img\insert-data.gif
[update-data]: img\update-data.gif
[delete-data]: img\delete-data.gif
[insert-data-courses]: img\insert-data-courses.gif
[insert-data-grades]: img\insert-data-grades.gif
