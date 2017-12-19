Task 1
------
1. Go to the `compose` directory, execute `docker-compose up` and go to `localhost:5000`. As you refresh the page, the number is being increased.
2. Parametrize the application to be executable in any environment with Redis installation.
3. Rename the service `redis` to `db`.


Task 2
------
1. Go to the `marathon` directory, execute `docker-compose up` and go to `localhost:8080`.
2. Schedule a new application named `test` - it's created from `nginx` image. Expose its TCP port 80.
3. Find out where the application is running (show the nginx page in your browser).
4. Scale the application to 2 instances and try to reach both instances.

 > Hint: The Docker container created by Marathon is running on the same Docker host as the Mesos/Marathon.
