Task 1
-------------
RabbitMQ is a popular messaging system but it's also something that you probably do not want to install on your personal computer. So using Docker to run RabbitMQ might be handy.

1. Find RabbitMB image on Docker Hub
2. Find an appropriate tag for 3.6 version with management inside
3. Run this image and forward exposed 15672 port to 8081
4. Put http://localhost:8081 to the browser and you should see RabbitMQ login screen
5. Try to see the running container using docker ps
6. Print out logs from the container using docker logs XXX

Task 2
-------------
Very simplified example of a new python app that you developed and now you need to run it in Docker. It contains a basic python web app using Flask. What will be interesting to you is that the webserver by default listens on port 5000.

1. Clone or download contents of this directory
2. You already have skeleton of Dockerfile, but it is not finished. Try to fill in blank parts - use the documentation page https://docs.docker.com/engine/reference/builder/
3. Build the image with tag my-first-application
4. Execute the image and publish the port as 8080
5. Execute the same image and publish the port as 8081
6. Login to you account on Docker Hub and push the image there
