Task 1
------
1. Go to the `compose` directory, execute `docker-compose up` and go to `localhost:5000`. As you refresh the page, the number is being increased.
2. Parametrize the application to be executable in any environment with Redis installation.
3. Rename the service `redis` to `db`.


Task 2
------
1. Go to the `marathon` directory, execute `docker-compose up` and go to `localhost:8080`.
2. Check that [marathon-lb](http://localhost:9090/haproxy?stats) works.
3. Schedule a new application named `test` - it's created from `nginx` image. Expose its TCP port 80 (bridge network).
4. Check in [marathon-lb](http://localhost:9090/haproxy?stats) that there is a new item related to the created service.
5. Find out where the application is running (show the nginx page in your browser).
6. Scale the application to 2 instances and try to reach both instances.

 > Hint: The Docker container created by Marathon is running on the same Docker host as the Mesos/Marathon, and `docker ps` is your friend.
