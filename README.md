# InterSCity Development Environment

This repository is composed of the scripts required to run all InterSCity's
microservices on the development environment. 
This project was tested in a GNU Linux Debian 8 and 9
environment.

## Dependencies

* Git
* [Docker (>= 1.13)](https://www.docker.com/)
* [Docker Compose (>= 1.10)](https://docs.docker.com/compose/)

## Setup

* Clone the repository
* Init submodules:
  `git submodule init`
* Update submodules:
  `git submodule update`
* Setup docker containers:
  `./project setup`

## Run the Development Environment

* Run the script:
  `./project start`

## Stop the Development Environment

* Run containers:
  `./project stop`

> OBS: One should always stop all microservices to avoid name and bind conflicts
Configure docker compose to run without root permission:

## Run tests

* You need to install shunit2 and moreutils package using the command:

    `$ apt-get install moreutils shunit2`

* To run all tests execute the command:

    `./project test`
