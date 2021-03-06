# SAL - Simplify After Lecture
## *Jude Javillo and Ronin Sharma*

Simplify After Lecture (SAL) is a one-stop online platform for simplifying all
of the different processes and services an educational course in the digital
age may need. Whether you need to hold office hours or organize online forums
for discussing challenging topics introduced during lecture, SAL has you 
covered! Forget about adding *another* site that students and faculty need to
learn how to use. SAL seeks to encompass all services that a typical college
course needs to properly educate its students effectively.

## Requirements

The main languages used for this application are Python and JavaScript. To
download all of the necessary requirements for Python, simply run 
`pip install -r requirements.txt`. As for JavaScript requirements, they should
all be encapsulated within the website's package dependencies, so navigate to 
the `website` directory and run `npm install`.

The database for SAL is MondoDB. SAL was developed using 5.0.6, so be sure to be
using at least MongoDB Community Server version 5.0.6.

## Development

Developing the different modules of SAL are relatively independent, thus come
with their own instructions. Each module is able to run on your local machine.
The following are instructions to get every module up and running to begin 
further development.

### Server

The server for SAL is written in Python, contained within the `server` 
directory. It uses Flask to simplify routing and increase development speed.
To run it, navigate to the `server` directory and execute the command 
`flask run`. Alternatively, from the top-level directory run the `Makefile`
command: `make run-server`. The server runs on port `8000`.

### Website

The website for SAL is written in JavaScript, contained within the `website`
directory. It uses React to simplify component creation. To run it, navigate to
the `website` directory and execute the command `npm run start`. Alternatively,
from the top-level directory run the `Makefile` command `make run-website`.
The website runs on port `9000`.

### Mobile

### Database

The database for SAL uses MongoDB and uses the `database` directory as its 
database path. To run it, navigate to the `database` directory and run 
`mongod --dbpath . --port 7000`. Alternatively, from the top-level directory
run the `Makefile` command `make run-database`. The database runs on port 
`7000`.

### Benchmark

### AWS

SAL is hosted on an AWS EC2 Instance. To connect to the development instance,
simply ssh into the cloud computer using the appropriate IP address as specified
by the admin AWS account. Alternatively, assuming that the correct address is
up-to-date in the `Makefile`, run `make run-aws`.

## Acknowledgements

SAL started as an MEng Project at Cornell University by Jude Javillo (CS MEng 
'22) and Ronin Sharma (ECE MEng '22) under the supervision of Professor
Christina Delimitrou.
