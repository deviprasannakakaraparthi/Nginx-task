Nginx proxy with docker 
This project tells how to run multiple services using docker and using one nginx revrese proxyu
It consists of 3 services:
Go service-A simple go web server application
Flask Service-Flask based Application
Nginx proxy 
All are exposed using same port that is 8020
How It Works
NGINX listens on port 8020 and uses path prefixes to route:
/service_1/ → to the Go app -port8001
/service_2/ → to the Flask app - port 8002
Docker Compose builds and starts all services together.
You can Acess the services-
	http://localhost:8020/service_1/hello
  http://localhost:8020/service_2/hello
How to run :
Clone the repo 
Run - docker-compose up --build
