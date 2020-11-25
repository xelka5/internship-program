# InternshipProgram Application

## Overview

The project contains 2 parts:

* UI Service written on Angular 9 (client side)
* API Service written on Spring Boot 2 (server side)

API service is connecting to the mysql server instance.
By default, admin user is created with credentials:

* `email: admin@internships.com`
* `password: testadmin`

## Usage

Postman test collections can be imported in local postman engine or can be executed directly from the docker container.

### Usage in docker

#### Supported docker environments

* DEV - environment used for testing final features, has swagger documentation and debugging support, postman tests are executed against it
* PROD - live production version, has disabled system endpoints, swagger docs and debugging, works inside encapsulated docker network

#### Running in docker

* To run PROD environment, execute `docker-compose up --build`
* To run DEV environment, execute `docker-compose -f docker-compose-dev.yml up --build`

### Running and developing locally

* Explained in readme files at service levels