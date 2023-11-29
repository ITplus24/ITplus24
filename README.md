# Getting Started with ITplus24

## Available Scripts

In the project directory, you can run:

### `docker-compose up --build`

this will build the necessery images and run backend, frontend, mongo and redis containers

## Web Application

visit http://localhost:3000

## Environemnt variables

to make it easy , I included the environemnt variables directly in the docker compose file
which is a bad choice

## Mails

since nodemailer has some issues when running inside a docker continer, I had to stop the send mails service
while running inside docker container

this can be done by the environemnt variable for backend service called ENVIRONEMT='docker'

thus it is still possible to send emails by assigning different value to the ENVIRONEMNT while running the backend service outside docker world
