# wordpress-mysql-phpmyadmin-docker
Easy WordPress development with Docker with default server Apache

With this project we can achive following:

* WordPress
* phpMyAdmin
* MySQL

Contents:

* Prerequisite
* Installation
* Usage

## Prerequisite 
Just make sure we have the latest versions of *Docker* and *Docker Compose* installed on your machine.

Clone this repository or copy the files from this repository into a new folder. In the docker-compose.yml file we can change the database host and database name as needed.

## Installation
Open a terminal and `cd` to the folder where docker-compose.yml is saved and run: `docker-compose up`
Here `volumes:`
* ./:/var/www/html - the location of your WordPress application (Full wordpress project)
* ./db_data:/var/lib/mysql - used to store and restore database dumps

## Usage
We can now use the up command:
`docker-compose up`
Use `-v` if we need to remove the database volume which is used to persist the database:

`docker-compose down -v`

## Finally
Visit `http://127.0.0.1:8000` to access WordPress project after starting the containers and

Visit `http://127.0.0.1:8080` to access phpMyAdmin after starting the containers.

