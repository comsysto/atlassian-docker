# Dockerbased Atlassian Environment
In this project we will set up an integrated environment of the Atlassian
development tools using Docker. The target is to have an easy way to bring up
an environment for demo purposes.

While it should also work for production this is not a use case we are eager to
support as Atlassian also does not. For production we suggest to deploy the
tools in a way that has support by Atlassian.

## Requirements
As everything will run on Docker it is required that Docker is installed. This
project was developed using Docker v1.9.1.

As we will configure our environment using it it is also required to have Docker
Compose installed. This project was developed using Docker Compose v1.5.2.

## Booting the environment
To make booting the environment easy a script called `startup.sh` is provided.
This script will invoke Docker Compose with the required parameter.

Please note that for the first time you boot up the environment an internet
connection is required as the Docker images have to be downloaded from
DockerHub. After this is done once everything should run on your local machine.

## Shutting down the environment
The running environment can be shutdown using `CTRL + C` in the console as
expected.
