Quick Start Guide

To run the application using docker container use following commands
docker run -d -p 3001:3001 -p 3000:3000 --name server daniyalmarghoob/neo-hackathon-vol4-cm15
Now you have containerized micro-service up and running.
Browse to http://localhost:3001 for application main route which responds simple "hello".
Browse to http://localhost:3001/swagger-stats/ui#sws_summary for dashboard.
In order to test the dashboard, use npm module loadtest. To import/download and execute loadtest use following commands
npm install -g loadtest
loadtest -c 10 --rps 2000 http://localhost:3001
You can visualize the increament in load using dashboard route.


